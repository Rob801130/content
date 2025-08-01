---
title: "HTML attribute: required"
short-title: required
slug: Web/HTML/Reference/Attributes/required
page-type: html-attribute
browser-compat:
  - html.elements.input.required
  - html.elements.select.required
  - html.elements.textarea.required
sidebar: htmlsidebar
---

The [Boolean](/en-US/docs/Glossary/Boolean/HTML) **`required`** attribute, if present, indicates that the user must specify a value for the input before the owning form can be submitted.

The `required` attribute is supported by `{{HTMLElement("input/text","text")}}`, `{{HTMLElement("input/search","search")}}`, `{{HTMLElement("input/url","url")}}`, `{{HTMLElement("input/tel","tel")}}`, `{{HTMLElement("input/email","email")}}`, `{{HTMLElement("input/password","password")}}`, `{{HTMLElement("input/date","date")}}`, `{{HTMLElement("input/month","month")}}`, `{{HTMLElement("input/week","week")}}`, `{{HTMLElement("input/time","time")}}`, `{{HTMLElement("input/datetime-local","datetime-local")}}`, `{{HTMLElement("input/number","number")}}`, `{{HTMLElement("input/checkbox","checkbox")}}`, `{{HTMLElement("input/radio","radio")}}`, `{{HTMLElement("input/file","file")}}`, {{HTMLElement("input")}} types along with the {{HTMLElement("select")}} and {{HTMLElement("textarea")}} form control elements. If present on any of these input types and elements, the {{cssxref(':required')}} pseudo class will match. If the attribute is not included, the {{cssxref(':optional')}} pseudo class will match.

The attribute is not supported on, or relevant to, {{HTMLElement("input/range","range")}} and {{HTMLElement("input/color","color")}} input types, as both have default values. Type `color` defaults to `#000000`. Type `range` defaults to the midpoint between `min` and `max` — with `min` and `max` defaulting to 0 and 100 respectively in most browsers if not declared. `required` is also not supported on the {{HTMLElement("input/hidden","hidden")}} input type — users cannot be expected to fill out a hidden form field. Finally, `required` is not supported on any button input types, including {{HTMLElement("input/image","image")}}.

In the case of a same named group of {{HTMLElement("input/radio","radio")}} buttons, if a single radio button in the group has the `required` attribute, a radio button in that group must be checked, although it doesn't have to be the one on which the attribute is applied. To improve code maintenance, it is recommended to either include the `required` attribute in every same-named radio button in the group, or else in none.

In the case of a same named group of {{HTMLElement("input/checkbox","checkbox")}} input types, only the checkboxes with the `required` attribute are required.

> [!NOTE]
> Setting [`aria-required="true"`](/en-US/docs/Web/Accessibility/ARIA/Reference/Attributes/aria-required) tells a screen reader that an element (any element) is required, but has no bearing on the optionality of the element.

### Attribute interactions

Because a read-only field cannot be changed, `required` does not have any effect on inputs with the [`readonly`](/en-US/docs/Web/HTML/Reference/Attributes/readonly) attribute also specified.

### Usability

When including the `required` attribute, provide a visible indication near the control informing the user that the {{HTMLElement("input")}}, {{HTMLElement("select")}} or {{HTMLElement("textarea")}} is required. In addition, target required form controls with the {{cssxref(':required')}} pseudo-class, styling them in a way to indicate they are required. This improves usability for sighted users. Assistive technology should inform the user that the form control is mandatory based on the required attribute, but adding `aria-required="true"` doesn't hurt, in case the browser / screen reader combination does not support `required` yet.

### Constraint validation

If the element is required and the element's value is the empty string, then the element is suffering from {{domxref('ValidityState.valueMissing','valueMissing')}} and the element will match the {{cssxref(':invalid')}} pseudo class.

## Accessibility concerns

Provide an indication to users informing them the form control is required. Ensure the messaging is multi-faceted, such as through text, color, markings, and attribute, so that all users understand the requirements whether they have color blindness, cognitive differences, or are using a screen reader.

## Example

### HTML

```html
<form>
  <div class="group">
    <input type="text" />
    <label>Normal</label>
  </div>
  <div class="group">
    <input type="text" required />
    <label>Required</label>
  </div>
  <input type="submit" />
</form>
```

### Result

{{EmbedLiveSample('Example')}}

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- {{domxref('validityState.valueMissing')}}
- {{cssxref(':required')}} and {{cssxref(':optional')}}
- {{htmlelement('input')}}
- {{htmlelement('select')}}
