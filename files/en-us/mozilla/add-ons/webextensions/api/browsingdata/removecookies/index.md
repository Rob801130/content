---
title: browsingData.removeCookies()
slug: Mozilla/Add-ons/WebExtensions/API/browsingData/removeCookies
page-type: webextension-api-function
browser-compat: webextensions.api.browsingData.removeCookies
sidebar: addonsidebar
---

Clears the browser's cookies.

You can use the `removalOptions` parameter, which is a {{WebExtAPIRef("browsingData.RemovalOptions")}} object, to:

- clear only cookies created after a given time
- control whether to clear cookies only set from normal web pages or to clear cookies set from hosted apps and extensions as well.

This is an asynchronous function that returns a [`Promise`](/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise).

## Syntax

```js-nolint
let removing = browser.browsingData.removeCookies(
  removalOptions            // RemovalOptions object
)
```

### Parameters

- `removalOptions`
  - : `object`. A {{WebExtAPIRef("browsingData.RemovalOptions")}} object, which may be used to clear only cookies created after a given time, and whether to clear cookies only set from normal web pages or to clear cookies set from hosted apps and extensions as well.

### Return value

A [`Promise`](/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise) that will be fulfilled with no arguments when the removal has finished. If any error occurs, the promise will be rejected with an error message.

## Examples

Remove cookies created in the last week:

```js
function onRemoved() {
  console.log("removed");
}

function onError(error) {
  console.error(error);
}

function weekInMilliseconds() {
  return 1000 * 60 * 60 * 24 * 7;
}

let oneWeekAgo = new Date().getTime() - weekInMilliseconds();

browser.browsingData
  .removeCookies({ since: oneWeekAgo })
  .then(onRemoved, onError);
```

Remove all cookies:

> [!WARNING]
> Using the API to remove all cookies will, simultaneously, clear all local storage objects (including those of other extensions).
>
> If you want to clear all cookies without disrupting local storage facilities, use [browser.cookies](/en-US/docs/Mozilla/Add-ons/WebExtensions/API/cookies) to loop through and remove the contents of all cookie stores.

```js
function onRemoved() {
  console.log("removed");
}

function onError(error) {
  console.error(error);
}

browser.browsingData.removeCookies({}).then(onRemoved, onError);
```

{{WebExtExamples}}

## Browser compatibility

{{Compat}}

> [!NOTE]
> This API is based on Chromium's [`chrome.browsingData`](https://developer.chrome.com/docs/extensions/reference/api/browsingData) API.

<!--
// Copyright 2015 The Chromium Authors. All rights reserved.
//
// Redistribution and use in source and binary forms, with or without
// modification, are permitted provided that the following conditions are
// met:
//
//    * Redistributions of source code must retain the above copyright
// notice, this list of conditions and the following disclaimer.
//    * Redistributions in binary form must reproduce the above
// copyright notice, this list of conditions and the following disclaimer
// in the documentation and/or other materials provided with the
// distribution.
//    * Neither the name of Google Inc. nor the names of its
// contributors may be used to endorse or promote products derived from
// this software without specific prior written permission.
//
// THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
// "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT
// LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR
// A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT
// OWNER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL,
// SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT
// LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
// DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY
// THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
// (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
// OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-->
