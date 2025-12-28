# Hosting Test - Vercel

This is a test of hosting a Hugo site on Vercel.

This site:

1. Includes content from a Hugo module
1. Transpiles Sass to CSS using Dart Sass
1. Performs vendor prefixing of CSS rules using the postcss, postcss-cli, and autoprefixer Node.js packages
1. Processes CSS files using the tailwindcss and @tailwindcss-cli Node.js packages
1. Encodes images to the WebP format
1. Includes a content file named hugö.md to verify that the Git `core.quotepath` setting is `false` [^1]

[^1]: See [issue #9810](https://github.com/gohugoio/hugo/issues/9810). Git's `core.quotepath` setting is `false` if `/tests/hugö` has a non-zero "last modified" date.

To simplify your setup and ensure you get the correct tool versions, it's a better practice to manage all build tool versions directly in your build script. This approach eliminates the need to split your settings between the dashboard and your project's code.
