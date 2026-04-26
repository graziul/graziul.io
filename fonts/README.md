# Fonts

Self-hosted variable fonts. All OFL-licensed.

Required files (download from sources below and place in this directory):

- `Newsreader-Variable.woff2` — variable upright (weight 200–800)
- `Newsreader-Italic-Variable.woff2` — variable italic (weight 200–800)
- `Inter-Variable.woff2` — variable upright (weight 100–900)
- `JetBrainsMono-Variable.woff2` — variable upright (weight 100–800)

## Sources

- **Newsreader:** https://github.com/productiontype/Newsreader (OFL). Or via Google Fonts → Get embed → use the variable static-host downloads.
- **Inter:** https://github.com/rsms/inter/releases (OFL). The `Inter.var.woff2` file from the release archive.
- **JetBrains Mono:** https://github.com/JetBrains/JetBrainsMono/releases (OFL). The `JetBrainsMono[wght].woff2` variable file from the release.

## Why self-host

- No third-party tracking via Google Fonts.
- Removes a request and a connection.
- Predictable load times.
- Brand-coherent with the privacy positioning in ADR-008.

## Fallback chain

If these files are missing, the `@font-face` rules in `src/styles/global.css` silently fall back to the next family in the stack — system serif/sans/mono — and the site still works. Visual changes only.

## Update cadence

Re-download once per year or when the upstream project ships a meaningful improvement. Pin versions in `_versions.txt` next to the woff2 files.
