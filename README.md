# .github

Organisation-level defaults for **net-flex** ([FlexSense](https://flexsense.co.uk)).

[`profile/README.md`](profile/README.md) is the public introduction rendered on
[github.com/net-flex](https://github.com/net-flex). GitHub only renders it while this
repository is **public** — everything committed here is world-readable, so nothing internal
belongs in it.

Internal machine setup and the repo catalogue live elsewhere, in a private repository.

## Editing the profile

Edit `profile/README.md` and push to `main`; the organisation page picks it up immediately.

It is deliberately a signpost, not a second website — one line on what FlexSense does, where
to go next, and what to expect from these repositories. Detail belongs on
[flexsense.co.uk](https://flexsense.co.uk), where it only has to be maintained once.

GitHub strips CSS from READMEs, so spacing comes from centred blocks and `<br>`. Check a
change through GitHub's own renderer before trusting it:

```sh
gh api markdown -X POST -f mode=gfm -f text="$(cat profile/README.md)"
```
