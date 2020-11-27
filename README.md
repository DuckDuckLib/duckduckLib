# DuckDuckLib

[toc]

## introduction

A Firefox extension that allows the user to search DuckDuckGo in a way which is identical to the usual DuckDuckGo search with two main exceptions:

1. **"Safe search" is disabled.** This is the main point of the extension. There will be one less algorithm deciding for you what is appropriate viewing. 

   Of course you may always use the [Safe Search page](https://safe.duckduckgo.com/) or change the settings on a per-search basis if for some reason you want this function. Read [about safe search](https://help.duckduckgo.com/duckduckgo-help-pages/features/safe-search/).

2. **Region-specific results are disabled**. Can be enabled on a per-search basis. Read [about regional search](https://help.duckduckgo.com/duckduckgo-help-pages/settings/regions/).

You do not need this extension to accomplish either of these goals. It is merely a convenience. 

## useage notes

### <!--Icon-->

<!--The **icon** used in the search bar is *slightly* different, so they it may be visually distinguished from the original.--> 

<!--Original DuckDuckGo icon-->

<!--![original DuckDuckGo](icons/icon-16.png)-->

<!--DuckDuckLib icon-->

<!--![dax-logo-lib-16](/Volumes/Five-Counter/CouldBeThis/duckducklib/icons/ddl-icon-16.png)-->

### omnibox search

the omnibox search is `ddl` so you can have regular duckduckgo (`ddg`) installed concurrently without interfering with it's behaviour. 

### Privacy

This extension merely formats your request from the location/search box to include the parameters described above DuckDuckGo. The information does not go anywhere else, or do anything other than it otherwise would. 

Please review DuckDuckGo's privacy policy: https://duckduckgo.com/privacy

## to do or consider

- [ ] investigate [`incognito` key in `manifest.json`](https://developer.mozilla.org/en-US/docs/Mozilla/Add-ons/WebExtensions/manifest.json/incognito) - should this be enabled?
- [ ] [`chrome_settings_overrides`](https://developer.mozilla.org/en-US/docs/Mozilla/Add-ons/WebExtensions/manifest.json/chrome_settings_overrides) could change home page to match 
- [ ] [Port a Google Chrome Extension](https://extensionworkshop.com/documentation/develop/porting-a-google-chrome-extension/)
- [ ] [Firefox for Android](https://www.mozilla.org/firefox/mobile/)
- [ ] allow configuration via options
- [ ] read:
  - [ ] [onboarding flow](https://extensionworkshop.com/documentation/develop/onboard-upboard-offboard-users/) 
  - [ ] [build an accessible extension](https://extensionworkshop.com/documentation/develop/build-an-accessible-extension/)

## sources & history

This extension is based on duckduckgo-safe by AdamVig, which does the exact opposite. It is available:

* install [firefox add-on from mozilla](https://addons.mozilla.org/en-US/firefox/addon/duckduckgo-safe/)
* see source on the [github repo](https://github.com/AdamVig/duckduckgo-safe)


DuckDuckGo logo/icon obtained from [their website](https://duckduckgo.com/assets/common/dax-logo.svg)

## liscence


![agplv3-with-text-162x68](/Volumes/Five-Counter/CouldBeThis/duckducklib/images/agplv3-with-text-162x68.png)

[Read all about it.](https://www.gnu.org/licenses/agpl-3.0.en.html)


