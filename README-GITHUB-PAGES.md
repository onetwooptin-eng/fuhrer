# EU-Fahrschule — GitHub Pages package

This folder is ready to publish as a static GitHub Pages website. Upload the
contents of this folder to the root of your GitHub repository; do not upload
the outer `github-ready-site` folder.

## Publish from GitHub

1. Create a repository and upload every file and folder in this package.
2. Open **Settings → Pages** in the repository.
3. Under **Build and deployment**, choose **Deploy from a branch**.
4. Select the `main` branch and the `/(root)` folder, then save.
5. In the **Custom domain** field, enter `eu-fahrschule.online`.
6. Add the DNS records shown by GitHub Pages at your domain provider, then
   enable **Enforce HTTPS** after the domain check succeeds.

The included `CNAME` file preserves the custom domain and `.nojekyll` tells
GitHub to publish the static files exactly as supplied.

## Activate the contact form

The old PHP mail handler has been replaced because GitHub Pages cannot run PHP.
The first test submission will send an activation message from FormSubmit to
`info@eu-fahrschule.online`. Open that message and confirm the form once. Then
submit the form again and verify that the enquiry arrives and redirects to the
thank-you page.

## Before going live

- Complete the operator address in `impressum/index.html`.
- Confirm that `robots.txt` and `sitemap.xml` open on the custom domain.
- Resubmit `https://eu-fahrschule.online/sitemap.xml` in Google Search Console.
- Keep the repository free of passwords, API keys, and server configuration.
