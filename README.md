# ITI-GIT-COURSE-LAB2

## Git Notes

### Delete Branches Locally

```bash
git branch -d dev
git branch -d test
```

Use `-D` instead of `-d` to force delete a branch:

```bash
git branch -D branch_name
```

### Delete Branches Remotely

```bash
git push origin --delete dev
git push origin --delete test
```

Or you can delete them directly from the GitHub website.

### Checkout Another Branch Without Committing Changes

**Option 1: Using stash (recommended)**

```bash
git stash
git checkout <other-branch>
git stash pop
```

This will save your uncommitted changes temporarily, switch to the other branch, then restore them.

**Option 2: Direct checkout**

```bash
git checkout <other-branch>
```

This works only if your changes don't conflict with the other branch.

### List All Tags

```bash
git tag
```

### Delete a Tag Locally and Remotely

```bash
git tag -d v1.7
git push origin --delete v1.7
```

### Add an Image in README

```markdown
![Alt text](path/to/image.png)
```

---

![Shakalelo](shakalelo.jpg)