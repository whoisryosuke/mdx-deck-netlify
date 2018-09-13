
# mdx-deck Template

A basic boilerplate to use with [mdx-deck](https://github.com/jxnblk/mdx-deck) with all components and layouts. Different themes and configurations available as feature branches.

[![Deploy to Netlify](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/whoisryosuke/mdx-deck-netlify)

## Features

Swap to different themes and configurations by building feature branches (or checkout + merge with production branch).

* [⚫ Dark theme](https://github.com/whoisryosuke/mdx-deck-netlify/tree/feat/dark-theme)

## Development

To run the presentation deck in development mode:

```sh
npm start
```

Edit the [`deck.mdx`](deck.mdx) file to get started.

## Exporting

To build the presentation deck as static HTML:

```sh
npm run build
```

To export a PDF:

```sh
npm run pdf
```

To export an image of the title slide:

```sh
npm run image
```

For more documentation see the [mdx-deck][] repo.

[mdx-deck]: https://github.com/jxnblk/mdx-deck

## Deploy

### Netlify

1. Clone the project locally and add to your Github
1. Add the repo to Netlify

or

1. Click deploy to Netlify on the example repo

## ⚙️ Netlify settings

In order to make sure our deck deploys properly using continuous integration, we have to configure Netlify to build and display our app.  

Go to your Deploy Settings (under the Deploys tab in your Netlify project/repo) and add the following settings:

1. Set the build script to `npm run build`
1. Set the deploy folder to `dist`

We give Netlify a build script to run each time we make a commit to the repo. And the deploy folder is the place where mdx-deck exports the static HTML/JS version, and by pointing Netlify there it displays our deck after building.

[See the demo site here](https://dazzling-kepler-4cc40d.netlify.com/)