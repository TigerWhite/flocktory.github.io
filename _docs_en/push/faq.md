---
layout: doc
title:  "FAQ"
section: push
---

### Before any problem

Check in cabinet settings→tracking→subdomain.
Check cabinet settings→SSL
For chrome, firefox check manifest added to site code head block:

```html
<link rel="manifest" href="/manifest.json">
```

### Does browser X support push?

Check [Browsers support]({{ site.baseurl }}{% link _docs_en/push/support.md %}). If browser not in list it not supported.

### Why I don't see push request on page?

Check [Browsers support]({{ site.baseurl }}{% link _docs_en/push/support.md %}).
Clean cookies and cache.
Remove from notification. Safari settings→notifications. Chrome chrome://settings/contentExceptions#notifications. Firefox TBD.

### I open page in incognito mode. I don't see push request. Why?

Push messages don't work in incognito mode.

### Which events widget sends?

Check [Push stats glossary]({{ site.baseurl }}{% link _docs_en/push/stats.md %}).

### Push opt-in works on my computer, but client see empty/wrong page. What happens?

This happens when client have outdated DNS cache on his computer or network hardware.
To clear cache on windows computer follow [this guide](https://technet.microsoft.com/en-us/library/64b84fc3-a7a1-44b4-b26b-596a643d066e).

### Chrome on http site open new window, but doesn't request push and doesn't close window. What to do?
Create new chrome profile and check again.
