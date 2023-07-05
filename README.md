# Retool Quickopen Extension

A Chrome extension to enable tab re-use of Retool. Inspired by a [similar extension](https://chrome.google.com/webstore/detail/zendesk-quicktab/moiloihigegdbekeabannnkibekfnekf) for Zendesk.

This extension is very basic and easy to customize for your use case:

1. `content-script.js` runs in the context of a web page. It scans the DOM for links to Retool, and modifies their click listener.
2. `service-worker.js` provides access to `chrome.tabs` APIs. This provides access to metadata on which tabs are open, and handles tab navigation.

## Install from source

1. `git clone https://github.com/tryretool/retool-quickopen-extension.git`
2. https://developer.chrome.com/docs/extensions/mv3/getstarted/development-basics/#load-unpacked