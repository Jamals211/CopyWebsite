# Shawn Jamal Blog

> Engineers & Economists

## Overview

This blog uses:

- [Eleventy](https://11ty.dev)
- [Static Site Generator (SSG)](https://staticgen.com)
- [Nunjucks](https://mozilla.github.io/nunjucks/)
- [Tailwind CSS](https://tailwindcss.com/)

## How to use

1. Clone this to a local repo.
2. Make appropriate changes to `/_data/metadata.json` and `_data/siteparams.json` to conform to your site’s parameters.
3. Run `npm install` to load all the dependencies in `package.json`, which includes Eleventy.
4. Run `npm run start` from your terminal app. You can then view the site in [http://localhost:3000](http://localhost:3000) on your computer.
5. Read the sample posts and their Markdown files to see how everything works.
6. Edit the content to make it your own!
7. When ready, [deploy the site](https://www.11ty.dev/docs/tutorials/#put-it-on-the-web) to your chosen host.

## What’s under the hood

- Lazy-loading of some images through use of [lazyload](https://github.com/verlok/vanilla-lazyload).
- Responsive images through my run-time `imgxfm.js` script and `lazypicture` shortcode.
- [PostCSS](https://postcss.org) and [Tailwind CSS](https://tailwindcss.com).
- Internal CSS in production mode, which is better for performance scores because it means one fewer [render-blocking resource](https://web.dev/render-blocking-resources/). In development mode, the CSS comes from a locally called `index.css` file, (**but** it’ll be a **huge** file, due to how Tailwind and [PurgeCSS](https://purgecss.com/) work in dev mode, so you may want to try using the experimental **[@tailwindcss/jit](https://github.com/tailwindlabs/tailwindcss-jit) library**; read more about it in [this announcement](https://blog.tailwindcss.com/just-in-time-the-next-generation-of-tailwind-css)); but don't worry about that now.

## Todo Checklist

A helpful checklist to gauge how your README is coming on what I would like to finish:

- [ ] Lots of items! :)

## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

1. Fork this repository;
2. Create your branch: `git checkout -b my-new-feature`;
3. Commit your changes: `git commit -m 'Add some feature'`;
4. Push to the branch: `git push origin my-new-feature`.

**After your pull request is merged**, you can safely delete your branch.

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for more information.
