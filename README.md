# Dev Util Info

## Table of Contents

* [VSCode](#vscode)
  * [Settings](#settings)
    * [File Exclusion](#file-exclusion)
    * [CodeLens](#codelens)
  * [Extensions](#extensions)
    * [Functional](#functional)
    * [Cosmetic](#cosmetic)
* [NPM](#npm)
  * [Global Packages](#global-packages)
    * [HTTP Server](#http-server)
    * [Angular CLI](#angular-cli)

## VSCode

### Settings

#### File Exclusion

Hides files/folders from the file explorer pane

```javascript
// settings.json
{
    // ...
    "files.exclude": {
        "**/.vs": true,
        "**/.vscode": true,
        "**/bin": true,
        "**/node_modules": true,
        "**/obj": true
    },
    // ...
}
```

#### CodeLens

Enables references for `.js`/`.ts` files

```javascript
// settings.json
{
    // ...
    "javascript.referencesCodeLens.enabled": true,
    "typescript.referencesCodeLens.enabled": true,
    "typescript.implementationsCodeLens.enabled": true,
    // ...
}

```

[Back to Top](#dev-util-info)

### Extensions

#### Functional

* [Angular 8 Snippets](https://marketplace.visualstudio.com/items?itemName=Mikael.Angular-BeastCode)

* C# - (probably already have this)

* [C# Extensions](https://marketplace.visualstudio.com/items?itemName=jchannon.csharpextensions)

  * Lets you right click a folder in the file explorer pane and
    create class/interface

* [Code Runner](https://marketplace.visualstudio.com/items?itemName=formulahendry.code-runner)

  * Lets you run code snippets (think dotnetfiddle)

* [Code Spell Checker](https://marketplace.visualstudio.com/items?itemName=streetsidesoftware.code-spell-checker)

* [Debugger for Chrome](https://marketplace.visualstudio.com/items?itemName=msjsdiag.debugger-for-chrome)

* [EditorConfig for VSCode](https://marketplace.visualstudio.com/items?itemName=EditorConfig.EditorConfig)

* [GitLens](https://marketplace.visualstudio.com/items?itemName=eamodio.gitlens)

  * Lots of git info (like for every line in a file you can see
    the last person who modified it and when)

* [Intellisense for CSS](https://marketplace.visualstudio.com/items?itemName=Zignd.html-css-class-completion)

* [Markdownlint](https://marketplace.visualstudio.com/items?itemName=DavidAnson.vscode-markdownlint)

* [Paste JSON as Code](https://marketplace.visualstudio.com/items?itemName=quicktype.quicktype)

  * Automagically generate a class from a JSON object

* [Path Intellisense](https://marketplace.visualstudio.com/items?itemName=christian-kohler.path-intellisense)

* [Remote - WSL](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-wsl)

  * Open folder in Windows Subsystem for Linux

* [TSLint](https://marketplace.visualstudio.com/items?itemName=ms-vscode.vscode-typescript-tslint-plugin)

* [vscode-solution-explorer](https://marketplace.visualstudio.com/items?itemName=fernandoescolar.vscode-solution-explorer)

  * Visual Studio style solution navigation

#### Cosmetic

* [Blueberry Banana](https://marketplace.visualstudio.com/items?itemName=pshershov.blueberry-banana)

  * Nifty color theme

* [Bracket Pair Colorizer](https://marketplace.visualstudio.com/items?itemName=CoenraadS.bracket-pair-colorizer)

  * Gives nested curly braces/bracket pairs different colors

* [GlassIt-VSC](https://marketplace.visualstudio.com/items?itemName=s-nlf-fh.glassit)

  * Adjust transparency of VSCode

* [Material Icon Theme](https://marketplace.visualstudio.com/items?itemName=PKief.material-icon-theme)

  * Better looking icons in file explorer

* [TODO Highlight](https://marketplace.visualstudio.com/items?itemName=wayou.vscode-todo-highlight)

  * Highlights TODO comments. Also lets you list all TODOs in your workspace

    * *NOTE:* You'll have to modify the `settings.json`

      ```javascript
      {
          // ...

          "todohighlight.include": [
              "**/*.js",
              "**/*.ts",
              "**/*.css",
              "**/*.scss",
              "**/*.sql",
              "**/*.cs",
              "**/*.md"
          ],

          // ...
      }

      ```

[Back to Top](#dev-util-info)

## NPM

### Global Packages

To list all currently installed global packages

`npm list -g --depth 0`

#### [HTTP Server](https://www.npmjs.com/package/http-server)

  Let's you spool up a server from command line in any folder

* Install

  `npm install -g http-server`

#### [Angular CLI](https://www.npmjs.com/package/@angular/cli)

* Install

  `npm install -g @angular/cli`

[Back to Top](#dev-util-info)
