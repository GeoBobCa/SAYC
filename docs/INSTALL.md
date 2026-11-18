# Add the lesson pilot to your SAYC site

1. In `2026-11-15_SAYC_Website`, merge the ZIP’s `docs` folder into your existing `docs` folder.
2. Open your existing `zensical.toml`. Paste the following entries immediately after the `Home` line inside `nav = [ ... ]`.

```toml
  { "Practice lessons" = [
    { "Minor support and a four-card major" = "lessons/bidding/minor-support-and-a-major.md" },
    { "Using a ruff as an entry" = "lessons/play/ruff-as-an-entry.md" },
  ] },
  { "From our games" = [
    { "November 16" = "from-our-games/2026-11-16/index.md" },
    { "Board 25" = "from-our-games/2026-11-16/board-25.md" },
    { "Board 16" = "from-our-games/2026-11-16/board-16.md" },
  ] },
```

3. From the site folder run `uv run zensical build --strict`. Preview with `uv run zensical serve`.
4. Open Practice lessons or From our games to try both lessons. Publish through your existing GitHub workflow when ready.

The HandViewer links open in new tabs. The alternative auction and club-ruff line are labelled separately from the recorded versions. The pilot uses the recorded November 16 deals. It does not require the central hand database.
