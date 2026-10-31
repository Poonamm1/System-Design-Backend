# System Design for Backend Engineers

GitHub always shows `.html` files as source in the repo. The live site is:

**[https://poonamm1.github.io/System-Design-Backend/](https://poonamm1.github.io/System-Design-Backend/)**

## Why the GitHub Action failed

`actions/configure-pages` cannot turn Pages on by itself. GitHub returns **404 Not Found** until Pages is enabled in the repo **Settings**. That is a GitHub account setting, not an HTML bug.

The Actions workflow was removed so commits no longer fail. This site is static (`index.html`), so GitHub can serve it **from the `main` branch**.

## Enable the live site (one time)

1. Make the repo **public** (Settings → General → Danger Zone → Change visibility). Free Pages does not work on a private repo without GitHub Pro.
2. Open **Settings → Pages**.
3. Under **Build and deployment**:
   - **Source:** Deploy from a branch
   - **Branch:** `main`
   - **Folder:** `/ (root)`
4. Click **Save**.
5. Wait about a minute, then open the link above.

You should see “Your site is live at …” on the Pages settings screen.
