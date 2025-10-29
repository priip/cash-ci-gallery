# Cash CI Gallery

Visual test gallery for UI and E2E test recordings from Cash iOS Buildkite builds.

**[View Gallery](https://priip.github.io/cash-ci-gallery)**

## 🧪 Current Process (Experimental)

*Experimental workflow to validate the concept*

1. **Buildkite on-demand job** records GIFs for UI/E2E tests
2. **Local extraction script** downloads artifacts and generates test data JSON
3. **Static HTML gallery** displays GIFs with filtering and build information

## 📁 File Structure

- `index.html` - Main gallery interface (HTML + CSS + JavaScript)
- `test-data.json` - Test metadata and build information
- `test-ownership.csv` - Module and team ownership mapping ([source](https://docs.google.com/spreadsheets/d/1u3hNvS6JQiBt9_ORCuZaR8IdUxvO-5-AV9utG_cyD9Y/edit?gid=457260210#gid=457260210))
- `gifs/` - Test recording GIFs

## 🚧 Next Steps

- **CI integration** - Automated extraction/publishing, possible integration with [#actionable-ci-results](https://www.notion.so/square-seller/Actionable-CI-Results-Home-go-actionable-ci-docs-27d70293beed80919ca8ccc7b897d739)
- **Storage & retention** - Where to store 500MB+ of GIFs per build? How many builds to keep?
- **Execution cadence** - Nightly? Per release? On-demand only?
- **Performance optimization** - Reduce GIF sizes? Use MP4s instead? Screenshots for frame-by-frame?
