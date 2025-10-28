# Cash CI Gallery

A web-based viewer for UI and E2E test artifacts from Cash iOS Buildkite builds.

## 🎯 Features

- **Visual test gallery** with iPhone-framed GIF recordings
- **Advanced filtering** by test type, module, team, and status
- **Real-time search** across test names, classes, and metadata
- **Statistics dashboard** with build information
- **Modal viewer** for detailed GIF inspection
- **Ownership mapping** from CSV data

## 🚀 View Live

[View the Gallery](https://YOUR_USERNAME.github.io/cash-ci-gallery)

## 📊 Data Structure

- `index.html` - Main gallery interface (HTML + CSS + JavaScript)
- `test-data.json` - Test metadata and build information
- `test-ownership.csv` - Module and team ownership mapping
- `gifs/` - Test recording GIFs

## 🛠️ Local Development

```bash
# Serve locally
python3 -m http.server 8001

# Open in browser
open http://localhost:8001
```

## 🎨 Design

Built with the Arcade design system for a native Cash App feel.
