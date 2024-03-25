# Bellutin

Bellutin forks from Bulletin, a minimal newsletter theme for [Ghost](https://github.com/TryGhost/Ghost). The theme divides your homepage into two sections. The left-hand section is optimized for capturing new email subscribers. I replaced its background color with the site cover. The right-hand section shows an excerpt from the latest issue you’ve published.

**Bulletin demo: https://bulletin.ghost.io**

# Instructions

1. [Download this theme](https://github.com/BilboTheHobbyist/bellutin/archive/main.zip)
2. Log into Ghost, and go to the `Design` settings area to upload the zip file
3. In the `Site wide` tab, set the `Background position` to crop the site cover in post menu.

# Development

Styles are compiled using Gulp/PostCSS to polyfill future CSS spec. You'll need [Node](https://nodejs.org/), [Yarn](https://yarnpkg.com/) and [Gulp](https://gulpjs.com) installed globally. After that, from the theme's root directory:

```bash
# Install
yarn

# Run build & watch for changes
yarn dev
```

Now you can edit `/assets/css/` files, which will be compiled to `/assets/built/` automatically.

The `zip` Gulp task packages the theme files into `dist/bulletin.zip`, which you can then upload to your site.

```bash
yarn zip
```
# Github actions (WIP)

## Ghost setup

1. In your online site adminsitration, click on `Integrations` menu
2. Click on the `Add custom integration` link
3. Give your integration a title such as `Github actions`
4. Copy the `Admin API key` and `Admin URL` field values 

## Github setup

1. Under your repository name, click on the `Settings` tab
2. In the left sidebar, click `Secrets`
3. On the right bar, click on `Add a new secret`
4. In the `Name` input box, type `GHOST_ADMIN_API_URL`
5. Type the value for your secret
6. Click Add secret
7. Reapeat for `GHOST_ADMIN_API_KEY` secret

# Contribution

If you're looking to contribute or raise an issue, head over to the main repository [TryGhost/Themes](https://github.com/TryGhost/Themes) where Ghost official themes are developed.

# Copyright & License

Copyright (c) bellerad.io - Released under the [MIT license](LICENSE).
