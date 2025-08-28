<div align="center">
  <img src="https://raw.githubusercontent.com/igorskyflyer/npm-biome-config/main/media/biome-config.png" alt="Icon of Config for Biome" width="256" height="256">
  <h1>Config for Biome</h1>
  <h4>By igorskyflyer (Igor Dimitrijević)</h4>
</div>

<br>

<h4 align="center">
  👽 An opinionated config for Biome to be used in JavaScript, TypeScript, JSX, TSX and any JavaScript-related projects. 🐺
</h4>

<br>
<br>

## 📃 Table of Contents

- [Features](#-features)
- [Usage](#-usage)
- [Changelog](#-changelog)
- [Support](#-support)
- [License](#-license)
- [Related](#-related)
- [Author](#-author)

<br>
<br>

## 🤖 Features

- ✅ Strict linting rules for **correctness**, **performance**, and **style**
- 🔄 **Auto-import** organization to maintain **clean** module structure
- 🎨 Custom **formatting** for **JSON** & **JavaScript**/**TypeScript** with **single** quotes, **LF** endings, and **space** indentation
- 🧠 **Complexity** warnings to reduce cognitive **overload** and improve logic **clarity**
- ⚡ **Performance**-focused rules blocking barrel files and re-export-all patterns
- 📁 Enforced **filenaming** **conventions** with strict casing and ASCII requirements
- 🛡️ **Suspicious** **behavior** checks including console usage, overload signatures, and error messaging
- ✒️ **Mo** **trailing** commas or **unnecessary** semicolons for **cleaner** output
- 🧹 Catches **unused** imports, variables, and class members before they **clutter** your codebase
- 🔍 **Supports** adjacent **overloads** & explicit length checks for **precise** **design** **patterns**

<br>
<br>

## 🕵🏼 Usage

Install it by executing any of the following, depending on your preferred package manager:

```bash
pnpm add -D @igorskyflyer/biome-config
```

```bash
yarn add -D @igorskyflyer/biome-config
```

```bash
npm i -D @igorskyflyer/biome-config
```

then extend the project's `biome.json` file from it, i.e.:

<br>

`biome.json`
```jsonc
{
  "$schema": "https://biomejs.dev/schemas/2.2.2/schema.json",
  "extends": ["@igorskyflyer/biome-config"]

  // Additional project-specific configuration
}
```

<br>
<br>

## 📝 Changelog

📑 The changelog is available here, [CHANGELOG.md](https://github.com/igorskyflyer/npm-biome-config/blob/main/CHANGELOG.md).

<br>
<br>

## 🪪 License

Licensed under the MIT license which is available here, [MIT license](https://github.com/igorskyflyer/npm-biome-config/blob/main/LICENSE).

<br>
<br>

## 💖 Support

<div align="center">
  I work hard for every project, including this one and your support means a lot to me!
  <br>
  Consider buying me a coffee. ☕
  <br>
  <br>
  <a href="https://ko-fi.com/igorskyflyer" target="_blank"><img src="https://raw.githubusercontent.com/igorskyflyer/igorskyflyer/main/assets/ko-fi.png" alt="Donate to igorskyflyer" width="180" height="46"></a>
  <br>
  <br>
  <em>Thank you for supporting my efforts!</em> 🙏😊
</div>

<br>
<br>

## 🧬 Related

[@igorskyflyer/zing](https://www.npmjs.com/package/@igorskyflyer/zing)

> _🐌 Zing is a C# style String formatter for JavaScript that empowers Strings with positional arguments - composite formatting. 🚀_

<br>

[@igorskyflyer/comment-it](https://www.npmjs.com/package/@igorskyflyer/comment-it)

> _📜 Formats the provided string as a comment, either a single or a multi line comment for the given programming language. 💻_

<br>

[@igorskyflyer/my-file-path](https://www.npmjs.com/package/@igorskyflyer/my-file-path)

> _🌟 An npm module that strongly types file paths! 🥊_

<br>

[@igorskyflyer/simple-exec](https://www.npmjs.com/package/@igorskyflyer/simple-exec)

> _🕺 Command. Execution. Made. Simple. ▶_

<br>

[@igorskyflyer/astro-easynav-button](https://www.npmjs.com/package/@igorskyflyer/astro-easynav-button)

> _🧭 Add an easy-to-use navigational button (jump to top/bottom) to your Astro site. 🔼_

<br>
<br>
<br>

## 👨🏻‍💻 Author
Created by **Igor Dimitrijević** ([*@igorskyflyer*](https://github.com/igorskyflyer/)).
