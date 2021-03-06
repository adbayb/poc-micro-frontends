<br>
<div align="center">
    <h1>๐งช Micro frontend runtime integration - single framework</h1>
    <strong>This POC aims to test a micro frontend runtime integration with the <a href="https://webpack.js.org/concepts/module-federation">module federation building block</a>.</strong>
</div>
<br>
<br>

## ๐ Quickstart

1๏ธโฃ Install by running:

```bash
pnpm i
```

2๏ธโฃ Try it by running:

```bash
npm start
```

<br>

## ๐ Architecture

<img alt="Micro frontend architectural diagram" src="https://user-images.githubusercontent.com/10498826/143263059-466a5261-aa7a-4ebb-b02c-e31db661f46e.png">

## ๐จ Module federation

The Webpack plugin `ModuleFederationPlugin` is used to configure federated modules builds and thier loading strategy at runtime.
All main available options are listed [here](https://github.com/webpack/webpack/blob/1c9b1b7a2136d4d9a27352fdbdf389490cca6460/types.d.ts#L6412) and documented [here](https://webpack.js.org/plugins/module-federation-plugin).

You can find configuration for the shell [here](shell/webpack.config.js) and one MFE [here](modules/absence/webpack.config.js).  

Other resources:
- [Module federation official website](https://module-federation.github.io/)
- [Webpack documentation](https://webpack.js.org/concepts/module-federation)
- [Getting out of version-mismatch-hell with module federation](https://www.angulararchitects.io/en/aktuelles/getting-out-of-version-mismatch-hell-with-module-federation/)
- [Interesting approach to manage resilient module federation integration with buildtime fallback](https://www.youtube.com/watch?app=desktop&v=K-yQB9YGmgE)
