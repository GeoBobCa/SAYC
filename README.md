# SAYC Bridge Reference

An editable Zensical reference for Standard American Yellow Card bidding, trick play, and defensive leads and signals.

## Preview on Windows

From the folder containing `zensical.toml`, run:

```powershell
uvx --from zensical==0.1.1 zensical serve
```

Open http://127.0.0.1:8000/. Use Ctrl+C in the terminal to stop the server. The first run may need to download Zensical. If you already have Zensical in an activated environment, use `zensical serve`.

## Edit and build

- Edit the Markdown pages in `docs/`. Keep the explicit anchor after a heading stable so that existing lesson links continue to work.
- Add new pages to the navigation list in `zensical.toml`.
- Use the site's **Linking lessons** page for examples of relative Markdown links and published paths.
- Run `uvx --from zensical==0.1.1 zensical build --clean` to regenerate `site/`. Publish the contents of that folder, with its directory structure intact. On GitHub Pages, the root of the Pages artifact should contain the generated `index.html`.
- Set `site_url` under `[project]` to the final published URL, including the repository path and trailing slash for a GitHub Pages project site, before the production build.

