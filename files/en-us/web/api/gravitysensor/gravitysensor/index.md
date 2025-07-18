---
title: "GravitySensor: GravitySensor() constructor"
short-title: GravitySensor()
slug: Web/API/GravitySensor/GravitySensor
page-type: web-api-constructor
browser-compat: api.GravitySensor.GravitySensor
---

{{securecontext_header}}{{APIRef("Sensor API")}}

The **`GravitySensor()`**
constructor creates a new {{domxref("GravitySensor")}} object which
provides on each reading the gravity applied to the device along all three axes.

## Syntax

```js-nolint
new GravitySensor()
new GravitySensor(options)
```

### Parameters

- `options` {{optional_inline}}
  - : Options are as follows:
    - `frequency` {{optional_inline}}
      - : The desired number of times per second a sample should
        be taken, meaning the number of times per second that the
        {{domxref('sensor.reading_event', 'reading')}} event will be called. A whole number or decimal may be
        used, the latter for frequencies less than a second. The actual reading frequency
        depends on device hardware and consequently may be less than requested. The default
        frequency is the one defined by the underlying platform.
    - `referenceFrame` {{optional_inline}}
      - : The local coordinate system representing
        the reference frame. It can be either `'device'` or
        `'screen'`. The default is `'device'`.

### Exceptions

- `SecurityError` {{domxref("DOMException")}}
  - : Use of this feature was blocked by a [Permissions Policy](/en-US/docs/Web/HTTP/Guides/Permissions_Policy).

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- {{domxref('sensor.reading_event', 'reading')}} event
