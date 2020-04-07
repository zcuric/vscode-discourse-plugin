# discourse-plugin-syntax-highlighting

[![vs-marketplace
version](https://badgen.net/vs-marketplace/v/zcuric.vscode-discourse-plugin)](https://marketplace.visualstudio.com/items?itemName=zcuric.vscode-discourse-plugin)
[![github license](https://badgen.net/github/license/zcuric/vscode-discourse-plugin)](https://github.com/zcuric/vscode-discourse-plugin/blob/master/LICENSE)

Syntax highlighting support for HTML `<script>` tags using `type="text/discourse-plugin"` which is actually javascript.

For example

```html
<script type="text/discourse-plugin">
  const settings = Discourse.SiteSettings,
    taggingEnabled = settings.tagging_enabled,
    title = settings.title;

  if (taggingEnabled) {
    console.log("Yay! "+title+" has tagging enabled!")
  } else {
    console.log("Ohh nooos! "+title+"Does not allow tagging.")
  }
</script>
```

More on discourse theme plugin development [here](https://meta.discourse.org/t/developer-s-guide-to-discourse-themes/93648).
