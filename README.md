<div align="center">
  <img src="https://raw.githubusercontent.com/igorskyflyer/npm-biome-config/main/media/biome-config.png" alt="Icon of Config for Biome" width="256" height="256">
  <h1>Config for Biome</h1>
</div>

<blockquote align="center">Strict Linting • Clean Imports • Consistent Style • Node ESM Ready</blockquote>

<h4 align="center">
  👽 An opinionated Biome configuration for modern JavaScript and TypeScript projects. Strict linting, consistent formatting, and performance-minded rules, all in one shareable config. 🐺
</h4>

<br>

## Table of Contents

- ✨ [**Features**](#features)
- 🕵🏼 [**Usage**](#usage)
- ⚙️ [**Implementation**](#implementation)
- 🎯 [**Motivation**](#motivation)
- 📝 [**Changelog**](#changelog)
- 🪪 [**License**](#license)
- 💖 [**Support**](#support)
- 🧬 [**Related**](#related)
- 👨🏻‍💻 [**Author**](#author)

<br>

## Features

- 👽 Strict linting rules for correctness, security, performance and style
- 🔍 Catches unused variables, imports, parameters and private class members
- 🎨 Custom formatting for `JSON` and `JS`/`TS` - single quotes, `LF` endings, 2-space indentation
- 🧠 Complexity rules to reduce cognitive load and improve logic clarity
- ⚡ Performance-focused rules - flags barrel files, re-export-all and top-level regex
- 📁 Enforced filenaming conventions with strict casing and `ASCII` requirements
- 🛡️ Security and suspicious checks - no dangerous patterns, console usage, overload signatures and error messaging
- ♿ Accessibility (a11y) warnings for JSX/HTML
- 🧪 Nursery (experimental) rules at warning level
- ✒️ Trailing commas in JS/TS (`all`) + no unnecessary semicolons for cleaner diffs
- 🧹 Import organization powered by Biome's built-in `organizeImports`
- 💎 Explicit length checks and adjacent overload signatures

<br>

## Usage

Install it by executing any of the following, depending on the preferred package manager:

```bash
bun add -D @igorskyflyer/biome-config
```

```bash
pnpm add -D @igorskyflyer/biome-config
```

```bash
yarn add -D @igorskyflyer/biome-config
```

```bash
npm i -D @igorskyflyer/biome-config
```

<br>

Then extend the config in **biome.json**:

`biome.json`
```json
{
  "extends": ["@igorskyflyer/biome-config"]
}
```

Override any rule locally as needed:

`biome.json`
```json
{
  "extends": ["@igorskyflyer/biome-config"],
  "linter": {
    "rules": {
      "suspicious": {
        "noConsole": "error"
      }
    }
  }
}
```

<br>

## Implementation

The config is split into three concern areas - formatting, linting and assist - each with deliberate, documented decisions.

**Formatting** enforces single quotes, no semicolons (`asNeeded`), trailing commas everywhere, 2-space indentation, `LF` line endings and `bracketSameLine: false` for clean prop/content separation in JSX and HTML attributes. JSON gets its own formatter section for consistency.

**Linting** enables eight rule groups with clear intent:
- **Correctness** - unused variables, imports, parameters and private class members
- **Security** - dangerous patterns (`error`)
- **Accessibility (a11y)** - JSX/HTML accessibility issues (`warn`)
- **Nursery** - experimental rules (`warn`)
- **Complexity** - simplified logic (`error`) and cognitive load warnings
- **Performance** - barrel files, re-export-all and top-level regex (`warn`)
- **Style** - filenaming (strictCase + ASCII), array literals, block statements, no Yoda expressions, etc.
- **Suspicious** - explicit `any`, console usage, error messaging and adjacent overload signatures

**Assist** enables Biome's built-in `organizeImports` for automatic, consistent import ordering on save.

<br>

## Motivation

Linting and formatting configurations are a source of endless inconsistency across projects. Each project ends up with its own slightly different `biome.json`, slightly outdated, with no single source of truth.

`@igorskyflyer/biome-config` solves this by providing one opinionated, versioned config that propagates across all projects via a simple `extends` - update once, apply everywhere.

<br>

## Changelog

Read about the latest changes in the [**CHANGELOG**](https://github.com/igorskyflyer/npm-biome-config/blob/main/CHANGELOG.md).

<br>

## License

Licensed under the [**MIT license**](https://github.com/igorskyflyer/npm-biome-config/blob/main/LICENSE).

<br>

## Support

<div align="center">
  Engineering and documenting open-source projects<br>
  involves a significant investment of time.
  <br><br>
  If this project or its implementation has provided value,<br>
  support is greatly appreciated.
  <br><br>
  <a href="https://ko-fi.com/igorskyflyer" target="_blank"><img src="https://raw.githubusercontent.com/igorskyflyer/igorskyflyer/main/assets/ko-fi.png" alt="Donate to igorskyflyer" width="180" height="46"></a>
  <br><br>
  <em>Thank you for supporting these efforts!</em> 🙏😊
</div>

<br>

## Related

This package is part of the [**dotfiles**](https://github.com/igorskyflyer/dotfiles) DX config suite - a curated index of independently installable configuration packages for linting, formatting, editing, JS/TS, React, Vue and many more.

### Other related packages

[**@igorskyflyer/zing**](https://www.npmjs.com/package/@igorskyflyer/zing)

> _🐌 Zing is a C# style String formatter for JavaScript that empowers Strings with positional arguments - composite formatting. 🚀_

[**@igorskyflyer/comment-it**](https://www.npmjs.com/package/@igorskyflyer/comment-it)

> _📜 Formats the provided string as a comment, either a single or a multi line comment for the given programming language. 💻_

[**@igorskyflyer/my-file-path**](https://www.npmjs.com/package/@igorskyflyer/my-file-path)

> _🌟 An npm module that strongly types file paths! 🥊_

[**@igorskyflyer/simple-exec**](https://www.npmjs.com/package/@igorskyflyer/simple-exec)

> _🕺 Command. Execution. Made. Simple. ▶_

[**@igorskyflyer/astro-easynav-button**](https://www.npmjs.com/package/@igorskyflyer/astro-easynav-button)

> _🧭 Add an easy-to-use navigational button (jump to top/bottom) to your Astro site. 🔼_

<br>

## Author
Created by **Igor Dimitrijević ([*@igorskyflyer*](https://github.com/igorskyflyer/))**.
