---
title: "ConstantSourceNode: ConstantSourceNode() constructor"
short-title: ConstantSourceNode()
slug: Web/API/ConstantSourceNode/ConstantSourceNode
page-type: web-api-constructor
browser-compat: api.ConstantSourceNode.ConstantSourceNode
---

{{APIRef("Web Audio API")}}

The **`ConstantSourceNode()`** constructor creates a new
{{domxref("ConstantSourceNode")}} object instance, representing an audio source which
constantly outputs samples whose values are always the same.

## Syntax

```js-nolint
new ConstantSourceNode(context, options)
```

### Parameters

- `context`
  - : An {{domxref("AudioContext")}} representing the audio context you want the node to
    be associated with.
- `options`
  - : A `ConstantSourceOptions` dictionary object defining the properties you
    want the `ConstantSourceNode` to have:
    - `offset`
      - : A read-only {{domxref("AudioParam")}} specifying the
        constant value generated by the source. The default is 1.0. The normal range is
        \-1.0 to 1.0, but the value can be anywhere in the range from
        `-Infinity` to `Infinity`.

## Examples

In this example, an audio context is created, then a `ConstantSourceNode` is
established with its `offset` initialized to 0.5.

```js
let audioContext = new AudioContext();

let myConstantSource = new ConstantSourceNode(audioContext, { offset: 0.5 });
```

> [!NOTE]
> The new `ConstantSourceNode` created by the
> constructor has a
> [`channelCount`](/en-US/docs/Web/API/AudioNode/channelCount) of
> 2\.

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}
