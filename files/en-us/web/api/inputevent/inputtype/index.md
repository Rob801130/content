---
title: "InputEvent: inputType property"
short-title: inputType
slug: Web/API/InputEvent/inputType
page-type: web-api-instance-property
browser-compat: api.InputEvent.inputType
---

{{APIRef("UI Events")}}

The **`inputType`** read-only property of the
{{domxref("InputEvent")}} interface returns the type of change made to editable content.
Possible changes include for example inserting, deleting, and formatting text.

## Value

A string containing the type of input that was made. There are many
possible values, such as `insertText`, `deleteContentBackward`,
`insertFromPaste`, and `formatBold`. For a complete list of the
available input types, see the [Attributes section of the Input Events Level 2 spec](https://w3c.github.io/input-events/#interface-InputEvent-Attributes).

## Examples

This example logs the `inputType` for [input events](/en-US/docs/Web/API/Element/input_event) on an editable
{{htmlElement("div")}}.

### HTML

```html
<p id="log">Input type:</p>
<div contenteditable="true" class="sample-text">
  <p>
    Some sample text. Try inserting line breaks, or deleting text in different
    ways, or pasting different content in.
  </p>
  <hr />
  <ul>
    <li>A sample</li>
    <li>bulleted</li>
    <li>list.</li>
  </ul>
  <p>Another paragraph.</p>
</div>
```

### CSS

```css
.sample-text {
  margin: 20px;
  padding: 20px;
  border: 2px dashed red;
}
```

### JavaScript

```js
const log = document.getElementById("log");
const editable = document.querySelector("div[contenteditable]");
editable.addEventListener("input", logInputType);

function logInputType(event) {
  log.textContent = `Input type: ${event.inputType}`;
}
```

### Result

Try editing the text inside the `<div>` and see what happens.

{{EmbedLiveSample("Examples", '100%', 500)}}

> [!NOTE]
> See also [Masayuki Nakano's InputEvent test suite](https://d-toybox.com/studio/lib/input_event_viewer.html) for a more detailed example.

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}
