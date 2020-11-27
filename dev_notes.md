## dev notes

ddg's [URL Parameter Reference Page](https://duckduckgo.com/params)

firefox [manifest.json keys](https://developer.mozilla.org/en-US/docs/Mozilla/Add-ons/WebExtensions/manifest.json)

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




info re omnibox for [developers](https://developer.mozilla.org/en-US/docs/Mozilla/Add-ons/WebExtensions/manifest.json/omnibox)

