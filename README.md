# Touareg Dev legal pages

Public, shared home for legal pages used by Touareg Dev apps. The GitHub repository slug is `touaregdevllc-legal-pages`; GitHub repository names cannot contain spaces.

## Published site

- Site home: <https://devtouareg07-eng.github.io/touaregdevllc-legal-pages/>
- Sands of Anubis privacy policy: <https://devtouareg07-eng.github.io/touaregdevllc-legal-pages/apps/sands-of-anubis/privacy-policy.html>
- Sands of Anubis terms of service: <https://devtouareg07-eng.github.io/touaregdevllc-legal-pages/apps/sands-of-anubis/terms-of-service.html>
- Sands of Anubis iOS privacy policy: <https://devtouareg07-eng.github.io/touaregdevllc-legal-pages/apps/sands-of-anubis-ios/privacy-policy.html>
- Sands of Anubis iOS terms of service: <https://devtouareg07-eng.github.io/touaregdevllc-legal-pages/apps/sands-of-anubis-ios/terms-of-service.html>
- Sands of Anubis iOS contact and support: <https://devtouareg07-eng.github.io/touaregdevllc-legal-pages/apps/sands-of-anubis-ios/contact-support.html>

GitHub Pages deploys the `site/` directory on each push to `main` through `.github/workflows/deploy-pages.yml`.

## Add another app

1. Create `site/apps/<app-slug>/` using lowercase letters and hyphens.
2. Copy `site/templates/privacy-policy.template.html` and `site/templates/terms-of-service.template.html` into that directory and rename them to `privacy-policy.html` and `terms-of-service.html`.
3. Replace every `[[...]]` placeholder. Describe the app's real data collection, storage, SDKs, ads, analytics, purchases, audience, retention, and contact method. Remove sections that do not apply and add any that do.
4. Link the app's two pages from its store listing and in-app settings, then verify both public URLs.
5. Add the new app to `site/index.html` and commit the changes to `main`.

The templates are drafting aids, not ready-to-publish policies or legal advice. Make each app's pages match its actual behavior and the laws that apply to it. They use the shared contact address `contact@touaregdev.com`; update it if an app needs a different contact.

## Structure

```text
site/
  index.html
  apps/
    sands-of-anubis/
      privacy-policy.html
      terms-of-service.html
    sands-of-anubis-ios/
      index.html
      privacy-policy.html
      terms-of-service.html
      contact-support.html
  assets/
    legal.css
  templates/
    privacy-policy.template.html
    terms-of-service.template.html
```
