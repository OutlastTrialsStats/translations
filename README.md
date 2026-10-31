# TOTStats Translations

Community translations for [OutlastTrialsStats](https://outlasttrialsstats.com), the stats platform for *The Outlast Trials*.

This repository holds only the texts of the website. Translating happens right here through pull requests, no
account on a translation platform needed and no developer skills required.

**Want to see TOTStats in your language? [Start here.](CONTRIBUTING.md)**

## Completeness

<!-- BEGIN COMPLETENESS TABLE -->
| Locale | Language | Translated | Complete |
| ------ | -------- | ---------- | -------- |
| `en-US` | English (source) | 1454 / 1454 | 100% |
| `it-IT` | Italian — Italiano | 1454 / 1454 | 100% |
| `zh-CN` | Chinese (Simplified) — 中文 | 1441 / 1454 | 99.1% |
| `ru-RU` | Russian — Русский | 766 / 1454 | 52.6% |
| `fr-FR` | French — Français | 749 / 1454 | 51.5% |
| `de-DE` | German — Deutsch | 733 / 1454 | 50.4% |
| `es-ES` | Spanish — Español | 729 / 1454 | 50.1% |
| `pl-PL` | Polish — Polski | 677 / 1454 | 46.5% |
| `ar-SA` | Arabic — العربية | 664 / 1454 | 45.6% |
| `tr-TR` | Turkish — Türkçe | 376 / 1454 | 25.8% |
<!-- END COMPLETENESS TABLE -->

Anything that is not translated yet (`null`) shows up in English on the website, so an incomplete language never
breaks anything.

## How it works

1. You edit the file of your language in [`locales/`](locales/) and open a pull request.
2. An automated check makes sure placeholders and formatting are intact.
3. Once a maintainer merges it, a pull request with your changes is opened in the website's repository and goes
   live with the next deployment.

`locales/en-US.json` is the source language. It comes from the website and new texts are added automatically.
You are welcome to correct typos or wording in it, but do not add or remove entries and keep every `{placeholder}`.

## For maintainers

```sh
node scripts/validate.mjs          # the checks CI runs
node scripts/validate.mjs --fix    # repair formatting, key order and missing keys
node scripts/status.mjs            # print the completeness table
node scripts/status.mjs --write-readme
```

Plain Node 20 or newer, no `npm install` needed.

## License

[MIT](LICENSE). Translations are contributed under the same license.
