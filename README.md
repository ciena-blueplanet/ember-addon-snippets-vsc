# ember-addon-snippets-vsc

Ember addon snippets for [VS Code](http://code.visualstudio.com/).

### Consuming ember addon snippets in VS Code
1. Launch the VS Code Command Pallete
2. Type `ext install ember-addon-snippets`
3. Note that there are 4 ways to trigger the snippets refreshal. I.e, to make the extension fetch the snippets from your opened project's addons.
  * restart vsc
  * reopen your project
  * Launch the VS Code Command Pallete and type `Ember: Refresh Snippets`
  * `cd` to your opened project and run `npm install` (Only works if it creates or modifies a `node_modules/ember-*/snippets/snippets.json`)
...

### Adding snippets to your ember addons

Follow these instructions to add snippets to your ember addons. It will ensure that they can be consumed by this extension in [VS Code](http://code.visualstudio.com/).

#### Handlebars snippets

1. Create a `snippets` folder at the root of your ember project.
2. Create a `vscode` folder inside the `snippets` folder.
2. Create a `handlebars.json` file inside the `vscode` folder.
3. Fill `./snippets/vscode/handlebars.json` with snippets. Your file should have the following format.

```json
{
    "frost-text": {
        "prefix": "frost-text",
        "body": "{{frost-text\n\tonInput=(action $1)\n}}\n$2"
    },
    "frost-textarea": {
        "prefix": "frosea",
        "body": "{{frost-textarea\n\tonInput=(action $1)\n}}\n$2"
    },
    "frost-password": {
        "prefix": "frost-password",
        "body": "{{frost-password\n\tonInput=(action $1)\n}}\n$2"
    },
    ...
}
```

#### Javascript snippets

1. Create a `snippets` folder at the root of your ember project.
2. Create a `vscode` folder inside the `snippets` folder.
2. Create a `javascript.json` file inside the `vscode` folder.
3. Fill `./snippets/vscode/javascript.json` with snippets. Your file should have the following format.

```json
{
    "Console Log": {
        "prefix": "log",
        "body": "console.log('$1')"
    },
    ...
}
```
