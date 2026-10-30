# TOTStats Translations

Community translations for [OutlastTrialsStats](https://outlasttrialsstats.com), the stats platform for *The Outlast Trials*.

This repository holds only the texts of the website. Translating happens right here through pull requests, no
account on a translation platform needed and no developer skills required.

**Want to see TOTStats in your language? [Start here.](CONTRIBUTING.md)**

## Completeness

<!-- BEGIN COMPLETENESS TABLE -->
| Locale | Language | Translated | Complete |
| ------ | -------- | ---------- | -------- |
| `en-US` | English (source) | 1453 / 1453 | 100% |
| `it-IT` | Italian — Italiano | 1453 / 1453 | 100% |
| `zh-CN` | Chinese (Simplified) — 中文 | 1440 / 1453 | 99.1% |
| `ru-RU` | Russian — Русский | 763 / 1453 | 52.5% |
| `fr-FR` | French — Français | 746 / 1453 | 51.3% |
| `de-DE` | German — Deutsch | 730 / 1453 | 50.2% |
| `es-ES` | Spanish — Español | 726 / 1453 | 49.9% |
| `pl-PL` | Polish — Polski | 674 / 1453 | 46.3% |
| `ar-SA` | Arabic — العربية | 661 / 1453 | 45.4% |
| `tr-TR` | Turkish — Türkçe | 201 / 1453 | 13.8% |
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
