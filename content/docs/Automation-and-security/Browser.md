---
bookCollapseSection: true
bookFlatSection: false
weight: 2
title: Browser vulnerability ✅
---

# Browser vulnerability

Daily we use browser to interact with different services. Some services require information on what device we use, what is our network connection, what is the hardware. The browser can give information on your location, to provide a website with relevant region data. The problem is that we don't know what data do we exactly share.

## Start with recommended checks

Go to [Privacy Analyzer](https://privacy.net/analyzer/) and go through the procedure.

![](../2020-06-23-14-25-41.png)

First step is giving us information about:

- IP address
- Geographical location
- Network provider
- Laptop and OS
- Browser version
- Screen resolution
- Battery life

![](../basic-info.png)

## If autofill can leak your data without you knowing about

In this example we can see that some geographical data is being shared automatically

![](../2020-06-23-14-30-11.png)

## Canvas fingerprint identifies your even without cookies

Systems identifies you with fingerprint, that consists from many variables and even if you try to hide them, it would be a chance it's you. You will have a unique fingerprint id that will be exchanges between other services to identify you.

![](../canvas-fingerprint.png)

Here are some more resource to go in deph with browser vulnerability checks

- [Panopticlick](https://panopticlick.eff.org/)
- [I am unique](https://amiunique.org/)
- [Browser audit](https://browseraudit.com/)