---
title: all
slug: Web/CSS/all
page-type: css-shorthand-property
browser-compat: css.properties.all
sidebar: cssref
---

The **`all`** [shorthand](/en-US/docs/Web/CSS/CSS_cascade/Shorthand_properties) [CSS](/en-US/docs/Web/CSS) property resets all of an element's properties except {{cssxref("unicode-bidi")}}, {{cssxref("direction")}}, and [CSS Custom Properties](/en-US/docs/Web/CSS/CSS_cascading_variables/Using_CSS_custom_properties). It can set properties to their initial or inherited values, or to the values specified in another cascade layer or stylesheet origin.

{{InteractiveExample("CSS Demo: all")}}

```css interactive-example-choice
/*no all property*/
```

```css interactive-example-choice
all: initial;
```

```css interactive-example-choice
all: inherit;
```

```css interactive-example-choice
all: unset;
```

```css interactive-example-choice
all: revert;
```

```html interactive-example
<section id="default-example">
  <div class="example-container-bg">
    <div class="example-container">
      <p id="example-element">
        This paragraph has a font size of 1.5rem and a color of gold. It also
        has 1rem of vertical margin set by the user-agent. The parent of the
        paragraph is a &lt;div&gt; with a dashed blue border.
      </p>
    </div>
  </div>
</section>
```

```css interactive-example
#example-element {
  color: gold;
  padding: 10px;
  font-size: 1.5rem;
  text-align: left;
  width: 100%;
}

.example-container {
  border: 2px dashed #2d5ae1;
}

.example-container-bg {
  background-color: #77767b;
  padding: 20px;
}
```

## Constituent properties

This property is a shorthand for all CSS properties except for {{cssxref("unicode-bidi")}}, {{cssxref("direction")}}, and [custom properties](/en-US/docs/Web/CSS/CSS_cascading_variables/Using_CSS_custom_properties).

## Syntax

```css
/* Global values */
all: initial;
all: inherit;
all: unset;
all: revert;
all: revert-layer;
```

The `all` property is specified as one of the CSS global keyword values. Note that none of these values affect the {{cssxref("unicode-bidi")}} and {{cssxref("direction")}} properties.

### Values

- {{cssxref("initial")}}
  - : Specifies that all the element's properties should be changed to their [initial values](/en-US/docs/Web/CSS/CSS_cascade/Value_processing#initial_value).
- {{cssxref("inherit")}}
  - : Specifies that all the element's properties should be changed to their [inherited values](/en-US/docs/Web/CSS/CSS_cascade/Inheritance).
- {{cssxref("unset")}}
  - : Specifies that all the element's properties should be changed to their inherited values if they inherit by default, or to their initial values if not.
- {{cssxref("revert")}}
  - : Specifies behavior that depends on the stylesheet origin to which the declaration belongs:
    - If the rule belongs to the [author origin](/en-US/docs/Web/CSS/CSS_cascade/Cascade#author_stylesheets), the `revert` value rolls back the [cascade](/en-US/docs/Web/CSS/CSS_cascade/Cascade) to the user level, so that the [specified values](/en-US/docs/Web/CSS/CSS_cascade/Value_processing#specified_value) are calculated as if no author-level rules were specified for the element. For purposes of `revert`, the author origin includes the Override and Animation origins.
    - If the rule belongs to the [user origin](/en-US/docs/Web/CSS/CSS_cascade/Cascade#user_stylesheets), the `revert` value rolls back the [cascade](/en-US/docs/Web/CSS/CSS_cascade/Cascade) to the user-agent level, so that the [specified values](/en-US/docs/Web/CSS/CSS_cascade/Value_processing#specified_value) are calculated as if no author-level or user-level rules were specified for the element.
    - If the rule belongs to the [user-agent origin](/en-US/docs/Web/CSS/CSS_cascade/Cascade#user-agent_stylesheets), the `revert` value acts like `unset`.
- {{cssxref("revert-layer")}}
  - : Specifies that all the element's properties should roll back the cascade to a previous [cascade layer](/en-US/docs/Web/CSS/@layer), if one exists. If no other cascade layer exists, the element's properties will roll back to the matching rule, if one exists, in the current layer or to a previous [style origin](/en-US/docs/Glossary/Style_origin).

## Formal definition

{{CSSInfo}}

## Formal syntax

{{csssyntax}}

## Examples

In this example, the CSS file contains styling for the {{HTMLElement("blockquote")}} element in addition to some styling for the parent `<body>` element. Various outputs in the Results subsection demonstrate how the styling of the `<blockquote>` element is affected when different values are applied to the `all` property inside the `blockquote` rule.

### HTML

```html
<blockquote id="quote">
  Lorem ipsum dolor sit amet, consectetur adipiscing elit.
</blockquote>
Phasellus eget velit sagittis.
```

### CSS

```css
body {
  font-size: small;
  background-color: #f0f0f0;
  color: blue;
  margin: 0;
  padding: 0;
}

blockquote {
  background-color: skyblue;
  color: red;
}
```

### Results

#### A. No `all` property

```html hidden
<blockquote id="quote">
  Lorem ipsum dolor sit amet, consectetur adipiscing elit.
</blockquote>
Phasellus eget velit sagittis.
```

```css hidden
body {
  font-size: small;
  background-color: #f0f0f0;
  color: blue;
}
blockquote {
  background-color: skyblue;
  color: red;
}
```

{{EmbedLiveSample("a._no_all_property", "200", "125")}}

This is the scenario in which no `all` property is set inside the `blockquote` rule. The {{HTMLElement("blockquote")}} element uses the browser's default styling which gives it a margin, together with a specific background and text color as specified in the stylesheet. It also behaves as a _block_ element: the text that follows it is beneath it.

#### B. `all: initial`

```html hidden
<blockquote id="quote">
  Lorem ipsum dolor sit amet, consectetur adipiscing elit.
</blockquote>
Phasellus eget velit sagittis.
```

```css hidden
body {
  font-size: small;
  background-color: #f0f0f0;
  color: blue;
}
blockquote {
  background-color: skyblue;
  color: red;
  all: initial;
}
```

{{EmbedLiveSample("b._all_initial", "200", "125")}}

With the `all` property set to `initial` in the `blockquote` rule, the {{HTMLElement("blockquote")}} element doesn't use the browser default styling anymore: it is an _inline_ element now (initial value), its [`background-color`](/en-US/docs/Web/CSS/background-color#formal_definition) is `transparent` (initial value), its [`font-size`](/en-US/docs/Web/CSS/font-size#formal_definition) is `medium`, and its [`color`](/en-US/docs/Web/CSS/color#formal_definition) is `black` (initial value).

#### C. `all: inherit`

```html hidden
<blockquote id="quote">
  Lorem ipsum dolor sit amet, consectetur adipiscing elit.
</blockquote>
Phasellus eget velit sagittis.
```

```css hidden
body {
  font-size: small;
  background-color: #f0f0f0;
  color: blue;
}
blockquote {
  background-color: skyblue;
  color: red;
  all: inherit;
}
```

{{EmbedLiveSample("c._all_inherit", "200", "125")}}

In this case, the {{HTMLElement("blockquote")}} element doesn't use the browser default styling. Instead, it inherits style values from its parent {{HTMLElement("body")}} element: it is a _block_ element now (inherited value), its {{cssxref("background-color")}} is `#F0F0F0` (inherited value), its {{cssxref("font-size")}} is `small` (inherited value), and its {{cssxref("color")}} is `blue` (inherited value).

#### D. `all: unset`

```html hidden
<blockquote id="quote">
  Lorem ipsum dolor sit amet, consectetur adipiscing elit.
</blockquote>
Phasellus eget velit sagittis.
```

```css hidden
body {
  font-size: small;
  background-color: #f0f0f0;
  color: blue;
}
blockquote {
  background-color: skyblue;
  color: red;
  all: unset;
}
```

{{EmbedLiveSample("d._all_unset", "200", "125")}}

When the `unset` value is applied to the `all` property in the `blockquote` rule, the {{HTMLElement("blockquote")}} element doesn't use the browser default styling. Because [`background-color`](/en-US/docs/Web/CSS/background-color#formal_definition) is a non-inherited property and [`font-size`](/en-US/docs/Web/CSS/font-size#formal_definition) and [`color`](/en-US/docs/Web/CSS/color#formal_definition) are inherited properties, the `<blockquote>` element is an _inline_ element now (initial value), its {{cssxref("background-color")}} is `transparent` (initial value), but its {{cssxref("font-size")}} is still `small` (inherited value), and its {{cssxref("color")}} is `blue` (inherited value).

#### E. `all: revert`

```html hidden
<blockquote id="quote">
  Lorem ipsum dolor sit amet, consectetur adipiscing elit.
</blockquote>
Phasellus eget velit sagittis.
```

```css hidden
body {
  font-size: small;
  background-color: #f0f0f0;
  color: blue;
}
blockquote {
  background-color: skyblue;
  color: red;
  all: revert;
}
```

{{EmbedLiveSample("e._all_revert", "200", "125")}}

When the `all` property is set to `revert` in the `blockquote` rule, the `blockquote` rule is considered to be non-existent and the styling property values are inherited from the ones applied to the parent element `<body>`. So the `<blockquote>` element gets styled as a _block_ element, with {{cssxref("background-color")}} `#F0F0F0`, {{cssxref("font-size")}} `small`, and {{cssxref("color")}} `blue` - all values inherited from the `body` rule.

#### F. `all: revert-layer`

```html hidden
<blockquote id="quote">
  Lorem ipsum dolor sit amet, consectetur adipiscing elit.
</blockquote>
Phasellus eget velit sagittis.
```

```css hidden
body {
  font-size: small;
  background-color: #f0f0f0;
  color: blue;
}
blockquote {
  background-color: skyblue;
  color: red;
  all: revert-layer;
}
```

{{EmbedLiveSample("f._all_revert-layer", "200", "125")}}

There are no cascade layers defined in the CSS file, so the `<blockquote>` element inherits its style from the matching `body` rule. The `<blockquote>` element here is styled as a _block_ element, with {{cssxref("background-color")}} `#F0F0F0`, {{cssxref("font-size")}} `small`, and {{cssxref("color")}} `blue` - all values inherited from the `body` rule. This scenario is an example of the case when `all` set to `revert-layer` behaves the same as when `all` is set to `revert`.

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

CSS global keyword values: {{cssxref("initial")}}, {{cssxref("inherit")}}, {{cssxref("unset")}}, {{cssxref("revert")}}, {{cssxref("revert-layer")}}
