# zyvorai organization profile

GitHub shows this content on **[github.com/zyvorai](https://github.com/zyvorai)** when published to the **`zyvorai/.github`** repository as `profile/README.md`.

This is **separate** from **[zyvorai/hypersdk](https://github.com/zyvorai/hypersdk)** `README.md`, which stays technical and Community Edition–focused.

## Publish

```bash
cd zyvorai-github
git add profile/README.md
git commit -m "Update organization profile README"
git push
```

If the repo doesn't exist yet:

```bash
gh repo create zyvorai/.github --public --description "Zyvor AI Labs GitHub organization profile" --source=. --remote=origin --push
```
