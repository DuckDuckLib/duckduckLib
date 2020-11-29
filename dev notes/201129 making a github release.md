# making a GitHub release

issue: [☑️ release v0.2 on github](https://github.com/CouldBeThis/duckduckLib/issues/7)

I had the idea that making a "release" on gh required an .xpi file because I have seen that before. So I did all this research. 

After this was done I went looking for example xpis from smaller developers and after going through over a dozen extension repos, wasn't able to find a single one. Most small extensions don't have a release at all, while others have code only. 

From looking at other ff add-on repos it looks like 3 files should be included:

- [ ] 1. Source code (zip) 
- [ ] 2. Source code (tar.gz) 
- [ ] 3. duckduckLib-signed.xpi

(1) and (2) are easy enough.

# creating an xpi file to upload to GitHub

issue: [☑️ creating an xpi file to upload to GitHub](https://github.com/CouldBeThis/duckduckLib/issues/6)

docs: [Submitting an add-on: self distribution (Web download)](https://extensionworkshop.com/documentation/publish/submitting-an-add-on/#self-distribution)

> make your extension available on a suitable web accessible server and when  the user downloads the signed add-on file Firefox will install it.

- [ ] need to add/check [`browser_specific_settings`](https://developer.mozilla.org/docs/Mozilla/Add-ons/WebExtensions/manifest.json/browser_specific_settings) in `manifest.json`
  - [ ] add/check [add-on id](https://extensionworkshop.com/documentation/develop/extensions-and-the-add-on-id/#When_do_you_need_an_add-on_ID) which is uuid: `{fd0fc302-032d-4e0b-9b8e-cf148aa123e9}`
  - [ ] "If you want Firefox to handle updates to your add-on", "`update_url` attribute set to point to an [update manifest file](https://developer.mozilla.org/Add-ons/Updates)"
- [ ] ensure it is updateable
  - [ ] create update manifest as described in [Updating your extension](https://extensionworkshop.com/documentation/manage/updating-your-extension/)
  - [ ] upload update manifest to GitHub
  - [ ] [test automatic updating](https://extensionworkshop.com/documentation/manage/updating-your-extension/#testing-automatic-updating)
- [ ] upload to [Submit a New Version](https://addons.mozilla.org/en-US/developers/addon/duckducklib/versions/submit/distribution?channel=listed) to distribute on my own
- [ ] download signed copy
- [ ] put on GitHub 

(Also an option: [Installing add-on from file](https://extensionworkshop.com/documentation/publish/distribute-sideloading) (sideloading) - don't see any reason for this)



















