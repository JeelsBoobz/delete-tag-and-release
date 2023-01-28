# GitHub Action: Delete tag and release

Add following step to your workflow:

```yaml
- uses: JeelsBoobz/delete-tag-and-release@latest
  with:
    tag_name: v0.1.0 #(required) tag name to delete 
    delete_release: true #(optional) default: true 
    repo: <owner>/<repoName> #(optional) target repository. default: repo running this action
  env:
    GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
```
