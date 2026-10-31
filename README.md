# System Design for Backend Engineers

GitHub always shows `.html` files as source in the repo. The live site is the rendered page.

**[Open the live HTML site](https://poonamm1.github.io/System-Design-Backend/)**

## One-time GitHub Pages setup

The first deploy failed because Pages was not enabled on this repository yet.

**Do this once on GitHub:**

1. Open the repo → **Settings** → **Pages**.
2. Under **Build and deployment** → **Source**, choose **GitHub Actions**.
3. If the repo is **private**, make it **public** (Pages on private repos needs GitHub Pro).
4. Re-run the failed **Deploy GitHub Pages** workflow: **Actions** → the failed run → **Re-run all jobs**.

After that, pushes to `main` publish the site automatically.
