---
title: "Permissions-Policy: usb directive"
short-title: usb
slug: Web/HTTP/Reference/Headers/Permissions-Policy/usb
page-type: http-permissions-policy-directive
status:
  - experimental
browser-compat: http.headers.Permissions-Policy.usb
sidebar: http
---

{{SeeCompatTable}}

The HTTP {{HTTPHeader("Permissions-Policy")}} header `usb` directive controls whether the current document is allowed to use the {{domxref("WebUSB API", "WebUSB API", "", "nocode")}}.

Specifically, where a defined policy blocks WebHID usage, the {{domxref("Navigator.usb")}} property will not be available.

## Syntax

```http
Permissions-Policy: usb=<allowlist>;
```

- `<allowlist>`
  - : A list of origins for which permission is granted to use the feature. See [`Permissions-Policy` > Syntax](/en-US/docs/Web/HTTP/Reference/Headers/Permissions-Policy#syntax) for more details.

## Default policy

The default allowlist for `usb` is `self`.

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- {{HTTPHeader('Permissions-Policy')}} header
- [Permissions Policy](/en-US/docs/Web/HTTP/Guides/Permissions_Policy)
