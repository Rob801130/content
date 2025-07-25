---
title: ::marker
slug: Web/CSS/::marker
page-type: css-pseudo-element
browser-compat: css.selectors.marker
sidebar: cssref
---

The **`::marker`** [CSS](/en-US/docs/Web/CSS) [pseudo-element](/en-US/docs/Web/CSS/Pseudo-elements) selects the marker box of a list item, which typically contains a bullet or number. It works on any element or pseudo-element set to [`display: list-item`](/en-US/docs/Web/CSS/display), such as the {{HTMLElement("li")}} and {{HTMLElement("summary")}} elements.

{{InteractiveExample("CSS Demo: ::marker", "tabbed-shorter")}}

```css interactive-example
li::marker {
  content: "✝ ";
  font-size: 1.2em;
}
```

```html interactive-example
<p>Group known as Mercury Seven:</p>
<ul>
  <li>Malcolm Scott Carpenter</li>
  <li>Leroy Gordon (Gordo) Cooper Jr.</li>
  <li>John Herschel Glenn Jr.</li>
  <li>Virgil Ivan (Gus) Grissom</li>
  <li>Walter Marty (Wally) Schirra Jr.</li>
  <li>Alan Bartlett Shepard Jr.</li>
  <li>Donald Kent (Deke) Slayton</li>
</ul>
```

## Allowable properties

The `::marker` pseudo-element supports a limited number of CSS properties, including:

- All [font properties](/en-US/docs/Web/CSS/CSS_fonts)
- The {{CSSxRef("white-space")}} property
- {{CSSxRef("color")}}
- {{CSSxRef("text-combine-upright")}}, {{CSSxRef("unicode-bidi")}}, and {{CSSxRef("direction")}} properties
- The {{CSSxRef("content")}} property
- All [animation](/en-US/docs/Web/CSS/CSS_animations#properties) and [transition](/en-US/docs/Web/CSS/CSS_transitions#properties) properties

> [!NOTE]
> The specification states that additional CSS properties may be supported in the future.

## Syntax

```css
::marker {
  /* ... */
}
```

## Examples

### HTML

```html
<ul>
  <li>Peaches</li>
  <li>Apples</li>
  <li>Plums</li>
</ul>
```

### CSS

```css
ul li::marker {
  color: red;
  font-size: 1.5em;
}
```

### Result

{{EmbedLiveSample('Examples')}}

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- HTML elements that have marker boxes by default: {{HTMLElement("ol")}}, {{HTMLElement("li")}}, {{HTMLElement("summary")}}
- [CSS generated content](/en-US/docs/Web/CSS/CSS_generated_content) module
- [CSS lists and counters](/en-US/docs/Web/CSS/CSS_lists) module
- [CSS counter styles](/en-US/docs/Web/CSS/CSS_counter_styles) module
