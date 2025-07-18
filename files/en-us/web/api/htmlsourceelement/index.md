---
title: HTMLSourceElement
slug: Web/API/HTMLSourceElement
page-type: web-api-interface
browser-compat: api.HTMLSourceElement
---

{{APIRef("HTML DOM")}}

The **`HTMLSourceElement`** interface provides special properties (beyond the regular {{domxref("HTMLElement")}} object interface it also has available to it by inheritance) for manipulating {{htmlelement("source")}} elements.

{{InheritanceDiagram}}

## Instance properties

_Inherits properties from its parent, {{domxref("HTMLElement")}}._

- {{domxref("HTMLSourceElement.height")}}
  - : A number that reflects the [`height`](/en-US/docs/Web/HTML/Reference/Elements/source#height) HTML attribute, indicating the height of the image resource in CSS pixels. The property has a meaning only if the parent of the current {{HTMLElement("source")}} element is a {{HTMLElement("picture")}} element.
- {{domxref("HTMLSourceElement.media")}}
  - : A string reflecting the [`media`](/en-US/docs/Web/HTML/Reference/Elements/source#media) HTML attribute, containing the intended type of the media resource.
- {{domxref("HTMLSourceElement.sizes")}}
  - : A string representing image sizes between breakpoints
- {{domxref("HTMLSourceElement.src")}}
  - : A string reflecting the [`src`](/en-US/docs/Web/HTML/Reference/Elements/source#src) HTML attribute, containing the URL for the media resource. The {{domxref("HTMLSourceElement.src")}} property has a meaning only when the associated {{HTMLElement("source")}} element is nested in a media element that is a {{htmlelement("video")}} or an {{htmlelement("audio")}} element. It has no meaning and is ignored when it is nested in a {{HTMLElement("picture")}} element.

    > [!NOTE]
    > If the `src` property is updated (along with any siblings), the parent {{domxref("HTMLMediaElement")}}'s `load` method should be called when done, since `<source>` elements are not re-scanned automatically.

- {{domxref("HTMLSourceElement.srcset")}}
  - : A string reflecting the [`srcset`](/en-US/docs/Web/HTML/Reference/Elements/source#srcset) HTML attribute, containing a list of candidate images, separated by a comma (`',', U+002C COMMA`). A candidate image is a URL followed by a `'w'` with the width of the images, or an `'x'` followed by the pixel density.
- {{domxref("HTMLSourceElement.type")}}
  - : A string reflecting the [`type`](/en-US/docs/Web/HTML/Reference/Elements/source#type) HTML attribute, containing the type of the media resource.
- {{domxref("HTMLSourceElement.width")}}
  - : A number that reflects the [`width`](/en-US/docs/Web/HTML/Reference/Elements/source#width) HTML attribute, indicating the width of the image resource in CSS pixels. The property has a meaning only if the parent of the current {{HTMLElement("source")}} element is a {{HTMLElement("picture")}} element.

## Instance methods

_No specific method; inherits methods from its parent, {{domxref("HTMLElement")}}._

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The HTML element implementing this interface: {{ HTMLElement("source") }}.
- The HTML DOM APIs of the elements that can contain a {{HTMLElement("source")}} element: {{domxref("HTMLVideoElement")}}, {{domxref("HTMLAudioElement")}}, {{domxref("HTMLPictureElement")}}.
