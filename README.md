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

Follow these [instructions](https://github.com/ciena-blueplanet/ember-addon-snippets/blob/master/README.md#adding-snippets-to-your-ember-addons) to add snippets compatible with this extension to your ember addons. 
