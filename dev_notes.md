# dev notes

[toc]

## duck duck go

ddg's [URL Parameter Reference Page](https://duckduckgo.com/params)

## firefox extension

### manifest.json

Firefox [manifest.json keys](https://developer.mozilla.org/en-US/docs/Mozilla/Add-ons/WebExtensions/manifest.json)

```
safe ON:	https://duckduckgo.com/?kp=1 
Safe Search: 	kp = 1 for On; kp = -1 for Moderate; kp = -2 for Off. 

safe:	https://duckduckgo.com/?q=TERM&t=h_&ia=web
unsafe:	https://duckduckgo.com/?q=TERM&kp=-2&t=h_&ia=web

https://duckduckgo.com/?kl=wt-wt&kp=-2
https://duckduckgo.com/?q=TERM&kl=wt-wt&kp=-2

```

only specifying safe search off:

```json
"search_url": "https://duckduckgo.com/?q={searchTerms}&kp=-2",
"suggest_url": "https://duckduckgo.com/ac/?q={searchTerms}&type=list",
```

also specifying no regional filters

```json
"search_url": "https://duckduckgo.com/?q={searchTerms}&kl=wt-wt&kp=-2",
"suggest_url": "https://duckduckgo.com/ac/?q={searchTerms}&kl=wt-wt&type=list",
```

[chrome_settings_overrides](https://developer.mozilla.org/en-US/docs/Mozilla/Add-ons/WebExtensions/manifest.json/chrome_settings_overrides)

> override certain browser settings. Two settings are available:
>
> - `"homepage"`, which enables you to override the browser's home page.
> - `"search_provider"`, which enables you to add a new search engine.

[OpenSearch description format](https://developer.mozilla.org/en-US/docs/Web/OpenSearch)

> lets a website describe a search engine for itself, so that a browser or other client application can use that search engine. 

### omnibox


info re omnibox for [developers](https://developer.mozilla.org/en-US/docs/Mozilla/Add-ons/WebExtensions/manifest.json/omnibox)

### packaging extension

#### web-ext

[Using web-ext](https://extensionworkshop.com/documentation/develop/getting-started-with-web-ext/#using-web-ext-section)

#### `lint`: basic error checking

```shell
web-ext lint
```

> Before trying out your extension with the [`run`](https://extensionworkshop.com/documentation/develop/web-ext-command-reference/#web-ext-run) command or submitting your package ... use the `lint` command to make sure your [manifest](https://developer.mozilla.org/Add-ons/WebExtensions/manifest.json) and other source files do not contain any errors.

[lint reference guide](https://extensionworkshop.com/documentation/develop/web-ext-command-reference/#web-ext-lint)

#### `run`: testing

```shell
web-ext run -o
```

`-o` = `--overwrite-dest`

> Overwrite destination package file if it exists. Without this option, web-ext will exit in error if the destination file already exists.

[run reference guide](https://extensionworkshop.com/documentation/develop/web-ext-command-reference/#web-ext-run) 

#### `build`: package

```shell
web-ext build
```

> This outputs a full path to the generated `.zip` file that can be loaded into a browser.

### dev community

- [Community Forums](https://discourse.mozilla.org/c/add-ons)

- [Email the community](https://mail.mozilla.org/listinfo/dev-addons)













