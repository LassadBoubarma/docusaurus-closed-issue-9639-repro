# Bug reproduction verification for (Closed) [Docusaurus Issue #9639](https://github.com/facebook/docusaurus/issues/9639)

This repository documents a reproduction attempt for a previously reported (now closed) issue in Docusaurus CLI related to specifying custom configuration files.

## 📝 Steps Clearly Followed to Verify:

### Step 1: Created a new Docusaurus site

```bash
npx create-docusaurus@latest my-website classic
cd my-website

2: Renamed the default configuration file
Renamed docusaurus.config.js to custom-config.js

Executed the Docusaurus CLI with custom configuration
The CLI threw the following clear and explicit error, consistent with the original issue’s reported:
[ERROR] Error: No config file found in site dir ``.
Expected one of:
- `docusaurus.config.ts`
- `docusaurus.config.mts`
- `docusaurus.config.cts`
- `docusaurus.config.js`
- `docusaurus.config.mjs`
- `docusaurus.config.cjs`
You can provide a custom config path with the `--config` option.

