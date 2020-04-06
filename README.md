# discourse-plugin-syntax-highlighting

Syntax highlighting support for HTML `<script>` tags using `type=text/discourse-plugin` which is actually javascript.

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
