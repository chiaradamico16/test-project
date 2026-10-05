# Adding your team via a pull request

**You'll need:** a GitHub account and [Git](https://git-scm.com/downloads) installed.

1. **Clone the repo:**
   ```bash
   git clone https://github.com/schmoigl/test-project.git
   cd test-project
   ```

2. **Create a branch:**
   ```bash
   git checkout -b add-team-yourteamname
   ```

3. **Edit `README.md`:** under "The Teams are:", write your team on an empty `- ` line and save the file.

4. **Commit and push:**
   ```bash
   git add README.md
   git commit -m "Add team <name>"
   git push -u origin add-team-yourteamname
   ```

5. **Open the PR:** on https://github.com/schmoigl/test-project, click **Compare & pull request** next to your branch. Check that the base is `main`, then click **Create pull request**.

**Merge conflict?** Another team probably edited the same lines. Run:

```bash
git pull origin main
```

Edit `README.md` so it keeps both teams and has no `<<<<<<<`, `=======` or `>>>>>>>` lines left. Then run `git add README.md`, `git commit`, and `git push`.
