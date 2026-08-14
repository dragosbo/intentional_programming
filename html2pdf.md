# HTML to PDF — Headless Browser Skill

Convert any local HTML file to a print-ready PDF using a Chromium-based browser in headless mode. No GUI, no print dialog, no dependencies to install.

## Command

### Microsoft Edge (Windows)

```cmd
"C:\Program Files (x86)\Microsoft\Edge\Application\msedge.exe" --headless --disable-gpu --print-to-pdf="output.pdf" "file:///C:/path/to/your/file.html"
```

### Google Chrome (Windows)

```cmd
"C:\Program Files\Google\Chrome\Application\chrome.exe" --headless --disable-gpu --print-to-pdf="output.pdf" "file:///C:/path/to/your/file.html"
```

### Chrome/Chromium (macOS/Linux)

```bash
google-chrome --headless --disable-gpu --print-to-pdf="output.pdf" "file:///home/user/path/to/file.html"
```

## How it works

1. The browser launches in headless mode (no visible window)
2. It loads the HTML file with full CSS/JS rendering
3. It prints to PDF using the same engine as `Ctrl+P` → "Save as PDF"
4. The process exits automatically

## Key flags

| Flag | Purpose |
|------|---------|
| `--headless` | Run without a visible browser window |
| `--disable-gpu` | Avoid GPU-related issues in headless mode |
| `--print-to-pdf="path"` | Output path for the generated PDF |
| `--no-pdf-header-footer` | Remove default header/footer (date, URL, page number) |
| `--print-to-pdf-no-header` | Same as above (Chrome 126+) |

## Tips

- **Use absolute paths** for both the output PDF and the input HTML file URI
- **File URIs use forward slashes** even on Windows: `file:///D:/folder/file.html`
- **Ignore error messages** — Edge/Chrome emit USB, sync, and renderer warnings that don't affect the output
- **CSS `@media print`** rules are respected — use them to hide nav elements or adjust layout for paper
- **Large files work fine** — the browser renders the full page before printing

## Example (this project)

```cmd
"C:\Program Files (x86)\Microsoft\Edge\Application\msedge.exe" --headless --disable-gpu --print-to-pdf="d:\work3\intentional_programming\intentional-programming.pdf" "file:///d:/work3/intentional_programming/intentional-programming.html"
```

## When to use this

- Generating PDFs from documentation or articles for offline reading
- Creating print-ready versions of HTML reports
- Automating PDF generation in CI/CD pipelines
- Sharing styled content with people who prefer PDF over HTML

## Alternatives

| Tool | Pros | Cons |
|------|------|------|
| Browser headless (this) | Zero install, full CSS support | Large file size |
| wkhtmltopdf | Lightweight, scriptable | Outdated rendering engine |
| Puppeteer (Node.js) | Programmable, fine-grained control | Requires Node.js |
| WeasyPrint (Python) | Good CSS support | Requires Python + install |
| Prince XML | Best print CSS support | Commercial license |
