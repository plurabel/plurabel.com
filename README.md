# plurabel.com

Built site only — the deploy artifact GitHub Pages serves.

**Canonical sources live in `~/cloud/git-projects/plurabel/docs/site/`**
(`github.com/plurabel/plurabel`). Rebuild and republish:

```text
cd ~/cloud/git-projects/plurabel
make site
cp -R docs/site/dist/. ~/cloud/git-projects/plurabel.com/
cd ~/cloud/git-projects/plurabel.com && git add -A && git commit -m "site: rebuild" && git push
```

Edit the sources, never this tree. See `docs/deploy-runbook.md` in the
source repo for DNS and host notes.
