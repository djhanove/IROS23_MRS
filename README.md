# IROS23_MRS_Workshop

IROS 2023 Workshop on Advances in Multi-Agent Learning - Coordination, Perception, and Control

## Local Development

1. **Install uv** (if needed):
   ```bash
   curl -LsSf https://astral.sh/uv/install.sh | sh
   ```

2. **Install dependencies:**
   ```bash
   uv sync --only-group docs
   ```

3. **Serve locally:**
   ```bash
   uv run --no-project mkdocs serve
   ```
   Open http://localhost:8000

4. **Build:**
   ```bash
   uv run --no-project mkdocs build
   ```

## Deployment

The site automatically deploys to GitHub Pages via GitHub Actions when you push to `main` or `master`.

To enable GitHub Pages:
1. Go to repository Settings → Pages
2. Set Source to "GitHub Actions"
