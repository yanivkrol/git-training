---
marp: true
paginate: true
footer: Natural Intelligence
---

# Git Collaboration

---

# Best practices

- Reviewing by commits
- Each commit should make sense on its own with a single purpose. E.g. a new a feature and a bug discovered when developing it should not be in the same commit.
  ```
  git commit -m "bug fix: ..."
  git commit -m "add support for ..."
  ```
- Use fixup commits to let the reviewer (and yourself) know what commits are you fixing.
- When development is finished, squash unnecessary commits before merging, will be easy and quick with `--autosquash` if using fixups.
- GitHub knows to display diffs even after overriding history, don't be afraid to `push -f` (when amending or rebasing)
