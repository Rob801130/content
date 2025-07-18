---
title: String.prototype.blink()
short-title: blink()
slug: Web/JavaScript/Reference/Global_Objects/String/blink
page-type: javascript-instance-method
status:
  - deprecated
browser-compat: javascript.builtins.String.blink
sidebar: jsref
---

{{Deprecated_Header}}

The **`blink()`** method of {{jsxref("String")}} values creates a string that embeds this string in a `<blink>` element (`<blink>str</blink>`), which used to cause a string to blink in old browsers.

> [!NOTE]
> All [HTML wrapper methods](/en-US/docs/Web/JavaScript/Reference/Global_Objects/String#html_wrapper_methods) are deprecated and only standardized for compatibility purposes. For the case of `blink()`, the `<blink>` element itself is removed from modern browsers, and blinking text is frowned upon by several accessibility standards. Avoid using the element in any way.

## Syntax

```js-nolint
blink()
```

### Parameters

None.

### Return value

A string beginning with a `<blink>` start tag, then the text `str`, and then a `</blink>` end tag.

## Examples

### Using blink()

The code below creates an HTML string and then replaces the document's body with it:

```js
const contentString = "Hello, world";

document.body.innerHTML = contentString.blink();
```

This will create the following HTML:

```html
<blink>Hello, world</blink>
```

> [!WARNING]
> This markup is invalid, because `blink` is no longer a valid element.

You should avoid blinking elements altogether.

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- [Polyfill of `String.prototype.blink` in `core-js`](https://github.com/zloirock/core-js#ecmascript-string-and-regexp)
- [es-shims polyfill of `String.prototype.blink`](https://www.npmjs.com/package/es-string-html-methods)
- [HTML wrapper methods](/en-US/docs/Web/JavaScript/Reference/Global_Objects/String#html_wrapper_methods)
