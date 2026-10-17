# dowse

A lightweight, cross-platform PDF reader with semantic search. Find passages by meaning, not just keywords. Runs fully offline.

> **Status:** Early planning. Nothing usable yet. Watch or star the repo to follow along.

## Why

`Cmd+F` / `Ctrl+F` only finds exact words. If you remember *what* a passage said but not *how* it was worded, you're stuck scrolling. dowse lets you search a PDF the way you remember it.

## Planned features

- **Semantic search:** search by meaning, with exact-keyword matches still supported (hybrid search)
- **Fast, lightweight reader:** small binary, no bundled browser
- **Annotations:** highlights, notes, and form filling, saved back to the PDF
- **Page tools:** reorder, rotate, delete, and merge pages
- **Library search:** search across all your PDFs, not just the open one
- **Fully offline:** the embedding model runs locally on your CPU, so your documents never leave your machine
- **Cross-platform:** macOS, Windows, and Linux

## How it will work

- **C++ core:** PDF parsing, text extraction, indexing, and search
- **Rendering:** [PDFium](https://pdfium.googlesource.com/pdfium/)
- **Embeddings:** a small quantized sentence-embedding model running on CPU
- **UI:** HTML/CSS/JS in the OS's native webview via [webview](https://github.com/webview/webview)

## Roadmap

- [ ] Minimal PDF parser: extract text from a page
- [ ] Webview window rendering pages with PDFium
- [ ] Keyword search with highlights
- [ ] Semantic search in the open document
- [ ] Annotations and incremental save
- [ ] Library-wide search
- [ ] Optional local "ask this PDF" mode

## Contributing

The project is in its early stages. Ideas and feedback are welcome in [Issues](../../issues).

## License

[MIT](LICENSE)
