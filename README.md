# github-actions-sample

## Trigger GitHub Actions with `repository_dispatch`

### Trigger GitHub Actions with `curl`

```shell
curl -X POST \
  -H "Accept: application/vnd.github+json" \
  -H "X-GitHub-Api-Version: 2022-11-28" \
  -H "Authorization: Bearer <YOUR-TOKEN>" \
  https://api.github.com/repos/mahata/github-actions-sample/dispatches \
  -d '{"event_type":"run-sample"}'
```

### Trigger GitHub Actions with `gh` CLI

```shell
gh api \
  --method POST \
  -H "Accept: application/vnd.github+json" \
  -H "X-GitHub-Api-Version: 2022-11-28" \
  /repos/mahata/github-actions-sample/dispatches \
   -f "event_type=run-sample"
```

---

test3
