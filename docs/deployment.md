# Deployment guide

This project is a static site: `index.html` is already the finished website. No build command, framework, or server is required.

Before deploying, open `index.html` locally, test both buttons, and check the privacy guidance in [SECURITY.md](../SECURITY.md).

## GitHub Pages

1. Create a new repository on GitHub.
2. Upload the project files, or push them with Git. Make sure `index.html` is at the repository root.
3. Open the repository on GitHub.
4. Go to **Settings → Pages**.
5. Under **Build and deployment**, choose **Deploy from a branch**.
6. Select your default branch (usually `main`) and the `/ (root)` folder.
7. Select **Save**.
8. Wait for GitHub to publish the site, then open the URL shown on the Pages settings screen.

The usual project-site address looks like `https://YOUR-USERNAME.github.io/YOUR-REPOSITORY/`. Publishing can take a few minutes. Push future changes to the selected branch to update the site.

## Netlify Drop

1. Visit [Netlify Drop](https://app.netlify.com/drop).
2. Sign in or create an account if requested.
3. Drag the entire project folder onto the drop area. The folder must contain `index.html` at its top level.
4. Wait for the upload and deployment to finish.
5. Open the generated site URL and test it.
6. In the Netlify dashboard, optionally choose a friendlier site name or connect a custom domain.

To publish an update with the manual Drop workflow, drag the updated folder into the site's deploy area again. Do not upload a folder that wraps the project in an extra directory level if Netlify cannot find `index.html`.

## Vercel

1. Push the project to a GitHub repository.
2. Sign in to [Vercel](https://vercel.com/).
3. Select **Add New → Project**.
4. Import the GitHub repository.
5. Leave the framework preset as **Other** (or no framework).
6. Leave the build command empty and use the repository root as the root directory.
7. Select **Deploy**.
8. Open the generated URL and test both desktop and mobile views.

Vercel redeploys automatically after new commits are pushed to the connected branch.

## After publishing

- Replace the live demo placeholder in `README.md` with the public URL.
- Add screenshots under `assets/screenshots/` and update the README paths.
- Test the public page without being signed in.
- Check that the repository contains no secrets or private personal details.
- Share the link respectfully and remove the page if someone featured in it withdraws consent.
