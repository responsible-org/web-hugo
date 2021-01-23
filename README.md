# Responsible.org Website

[![Netlify Status](https://api.netlify.com/api/v1/badges/12828934-d238-42ed-beaf-c9de1e5c8c23/deploy-status)](https://app.netlify.com/sites/zen-ardinghelli-8cc957/deploys)
We are deployed on Netlify using Forester CMS for content with and use
Themefisher and the new Hugo module support that pulls from their repo

To snapshot those modules, you can use
[Hugo](https://gohugo.io/commands/hugo_mod_vendor/) to do this with a single
command which adds all the modules currently running and puts them into
[_vendor](_vendor);

```bash
hugo mod gen
```
The images here are actually imported from the theme. To override and add yur
own images, you need to create a image directory.

## Based on  Hugo Parsa Forestry Starter

[Hugo Parsa Theme developed by
Themefischer](https://github.com/themefisher/parsa-hugo) for Forestry CMS.

![Parsa Theme Preview](static/images/screenshot.jpg)

Import to Forestry in one single click!

[![Import to Forestry](https://assets.forestry.io/import-to-forestryK.svg)](https://app.forestry.io/quick-start?repo=forestryio/hugo-parsa-forestry&engine=hugo&version=0.74.3)

## Prerequisites

- Hugo > 0.62.2 (tested with 0.74.3)

## Content Management

![Forestry user interface](static/images/hugo-parsa-forestry.jpg)

This project has been pre-configured to work with
[Forestry](https://forestry.io), just import your repository ✨. \ Any changes
you make will be commited back to the repo, and deployed if you're using
Netlify.

## Customization

You can customize the theme through the [`config.toml`
file](https://github.com/forestryio/hugo-parsa-forestry/blob/master/config.toml).
Those values are accessible from within Forestry.

## Deployment and hosting with Netlify

Import your site in [Netlify](https://netlify.com)

1. Create a new site in Netlify and import your repository.
2. Set the build command to: `hugo --gc --minify`
3. Set the publish directory to: `public`
4. Set `HUGO_VERSION` to `0.74.3`

That's it, now your site gets deployed automatically on `git push` or when
saving documents from Forestry.

## Development

```bash
# clone your repository
# cd in the project directory
cd hugo-parsa-forestry

# Start local dev server
hugo server
```

For more information, see [official Hugo documentation](https://gohugo.io/getting-started/).
