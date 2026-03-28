# Pages Root Layout

Use the contents of this directory as the root of your GitHub Pages site for Universal Links.

This layout is correct for either:

- a user site repo named `neonko.github.io`
- a custom domain pointed at GitHub Pages

It is not sufficient to publish the current `neonko/OpenGlasses` repository as a project site, because Apple expects:

- `https://neonko.github.io/.well-known/apple-app-site-association`

while a project site publishes under:

- `https://neonko.github.io/OpenGlasses/...`

Expected deployed paths:

- `/.well-known/apple-app-site-association`
- `/OpenGlasses/index.html`

Recommended setup:

1. Create a separate repository named `neonko.github.io`.
2. Copy the contents of this directory to the root of that repository.
3. Publish the `main` branch with GitHub Pages.
4. Keep the app settings as:
   - Team ID: `692K79G242`
   - Bundle ID: `io.github.neonko.openglasses`
   - Universal Link URL: `https://neonko.github.io/OpenGlasses`
