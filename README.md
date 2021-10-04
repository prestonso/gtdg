# _Gatsby: The Definitive Guide_ code examples

Welcome to the code examples repository for the book _[Gatsby: The Definitive Guide](https://www.oreilly.com/library/view/gatsby-the-definitive/9781492087502/)_ (O'Reilly, 2021) by [Preston So](https://preston.so)! This repository contains information about and references to other repositories that represent working implementations found in the book for the benefit of readers, though it does not contain any code itself apart from this README file.

Because Gatsby as a framework and the surrounding JavaScript landscape is evolving rapidly, some code examples may be out of date or otherwise contain errors. Errata for code examples can be found below the list of code repositories below. To report an issue with these code examples, please open an issue in the respective repository or [contact the author](https://preston.so/contact). To report an issue with the Gatsby framework, please open an issue in the [official Gatsby repository](https://github.com/gatsbyjs/gatsby).

You can find more information about Gatsby at [the Gatsby website](https://gatsbyjs.com).

## Repositories

Repositories containing code examples are listed below in the order in which they appear in the book _Gatsby: The Definitive Guide_. Some examples from the book are excluded because they are purely demonstrative or illustrative rather than representative of a production-ready Gatsby codebase. For errata on these repositories, consult the _Errata_ section below.

| Repository | Chapter | Page number |
| --- | --- | --- |
| `[gtdg-ch2-pages-components](https://github.com/prestonso/gtdg-ch2-pages-components)` | Chapter 2: Core Elements of Gatsby | 38 |
| `[gtdg-ch2-global-styling-with-layout](https://github.com/prestonso/gtdg-ch2-global-styling-with-layout)` | Chapter 2: Core Elements of Gatsby | 47 |
| `[gtdg-ch2-global-styling-without-layout](https://github.com/prestonso/gtdg-ch2-global-styling-without-layout)` | Chapter 2: Core Elements of Gatsby | 48 |
| `[gtdg-ch2-css-in-js-emotion](https://github.com/prestonso/gtdg-ch2-css-in-js-emotion)` | Chapter 2: Core Elements of Gatsby | 52 |
| `[gtdg-ch2-css-in-js-styled-components](https://github.com/prestonso/gtdg-ch2-css-in-js-styled-components)` | Chapter 2: Core Elements of Gatsby | 55 |
| `[gtdg-ch3-features](https://github.com/prestonso/gtdg-ch3-features)` | Chapter 3: Adding Features to Gatsby Sites | 68 |
| `[gtdg-ch4-graphql](https://github.com/prestonso/gtdg-ch4-graphql)` | Chapter 4: GraphQL and the Gatsby Data Layer | 109 |
| `[gtdg-ch6-programmatic-pages](https://github.com/prestonso/gtdg-ch6-programmatic-pages)` | Chapter 6: Programmatic Page Creation | 170 |
| `[gtdg-ch7-importing-assets](https://github.com/prestonso/gtdg-ch7-importing-assets)` | Chapter 7: Assets in Gatsby | 193 |
| `[gtdg-ch7-gatsby-plugin-image](https://github.com/prestonso/gtdg-ch7-gatsby-plugin-image)` | Chapter 7: Assets in Gatsby | 203 |
| `[gtdg-ch7-gatsby-image](https://github.com/prestonso/gtdg-ch7-gatsby-image)` | Chapter 7: Assets in Gatsby | 209 |
| `[gtdg-ch8-algolia](https://github.com/prestonso/gtdg-ch8-algolia)` | Chapter 8: Adding Data-Driven Features to Gatsby Sites | 225 |
| `[gtdg-ch8-commenting](https://github.com/prestonso/gtdg-ch8-commenting)` | Chapter 8: Adding Data-Driven Features to Gatsby Sites | 229 |
| `[gtdg-ch8-taxonomy-pagination](https://github.com/prestonso/gtdg-ch8-taxonomy-pagination)` | Chapter 8: Adding Data-Driven Features to Gatsby Sites | 231 |
| `[gtdg-ch8-rss](https://github.com/prestonso/gtdg-ch8-rss)` | Chapter 8: Adding Data-Driven Features to Gatsby Sites | 243 |
| `[gtdg-ch8-authentication](https://github.com/prestonso/gtdg-ch8-authentication)` | Chapter 8: Adding Data-Driven Features to Gatsby Sites | 248 |
| `[gtdg-ch9-plugin](https://github.com/prestonso/gtdg-ch9-plugin)` | Chapter 9: Gatsby Plugins and Starters | 267 |
| `[gtdg-ch9-example-site](https://github.com/prestonso/gtdg-ch9-example-site)` | Chapter 9: Gatsby Plugins and Starters | 277 |
| `[gtdg-ch9-source-plugin](https://github.com/prestonso/gtdg-ch9-source-plugin)` | Chapter 9: Gatsby Plugins and Starters | 277 |
| `[gtdg-ch10-using-themes](https://github.com/prestonso/gtdg-ch10-using-themes)` | Chapter 10: Gatsby Themes | 313 |
| `[gtdg-ch10-theme-shadowing](https://github.com/prestonso/gtdg-ch10-theme-shadowing)` | Chapter 10: Gatsby Themes | 328 |
| `[gtdg-ch11-unit-testing](https://github.com/prestonso/gtdg-ch11-unit-testing)` | Chapter 11: Testing and Debugging Gatsby | 336 |
| `[gtdg-ch13-mdx](https://github.com/prestonso/gtdg-ch13-mdx)` | Chapter 13: Advanced Topics in Gatsby | 385 |

## Errata

### `[gtdg-ch9-source-plugin](https://github.com/prestonso/gtdg-ch9-source-plugin)`

As of v3, the `[node-fetch](https://www.npmjs.com/package/node-fetch)` package no longer supports `require()`, which impacts the `gatsby-node.js` file in the `gtdg-ch9-source-plugin` example. However, v2 is still supported. As a quick fix, replace the command on page 281 of _Gatsby: The Definitive Guide_ with the following instead, paying close attention to the `@2.6.5` suffix after `node-fetch`:

```
$ npm install apollo-cache-inmemory apollo-client apollo-link apollo-link-http apollo-link-ws apollo-utilities graphql graphql-tag node-fetch@2.6.5 ws subscriptions-transport-ws
```

To use `node-fetch@3.0.0` or higher, consult the `node-fetch` documentation for information about [loading and configuring the module](https://www.npmjs.com/package/node-fetch#loading-and-configuring-the-module).
