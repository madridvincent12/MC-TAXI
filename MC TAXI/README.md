# MC Taxi Daily Income Tracker

A simple mobile-first web app for tracking daily taxi earnings, with an automatic 20% MC Taxi commission calculation. Data is saved in the browser (localStorage).

## Deploy with GitHub Pages
1. Create a new repository on GitHub (for example `mc-taxi-tracker`).
2. Upload `index.html`, `.nojekyll` and `README.md` to the repository root.
3. Go to Settings > Pages. Under "Build and deployment", set Source to "Deploy from a branch", choose the `main` branch and the `/ (root)` folder, then Save.
4. After a minute or two your app is live at `https://<your-username>.github.io/mc-taxi-tracker/`.

Open that link on your phone and use "Add to Home Screen" to launch it like an app.

## Login
Default account: username `Admin`, password `Admin` (username is not case-sensitive, password is). Change the password in the app with "Change password". This is a simple on-device lock, not server-side security.

## Tips and commission
The commission rate (default 20%) can be changed in the app. Tips are entered separately with ADD TIP: they have no commission and are added straight to net earnings.

## Expenses
Gasoline and other fees are added with ADD GAS and ADD FEE. They are deducted from your take-home: net = fares - commission + tips - gasoline - other fees. Commission is calculated on fares only.
