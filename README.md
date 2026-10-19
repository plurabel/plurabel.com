# plurabel.com

The built website for [Plurabel](https://github.com/plurabel/plurabel), a small imprint of one-job apps for iPhone and Mac. This repository holds only the generated site that GitHub Pages serves. Do not edit it by hand.

## Where the source is

The site is written in the `docs/site/` folder of the [plurabel/plurabel](https://github.com/plurabel/plurabel) repository. To rebuild and republish it, from a checkout of that repository with this one cloned beside it as `../plurabel.com`:

```text
make site
cp -R docs/site/dist/. ../plurabel.com/
cd ../plurabel.com
git add -A
git commit -m "site: rebuild"
git push
```

Expected: `make site` writes the built pages to `docs/site/dist`; after the push, GitHub Pages republishes the site. DNS and host notes are in `docs/deploy-runbook.md` in the source repository.

## License

All rights reserved until a license is chosen.
