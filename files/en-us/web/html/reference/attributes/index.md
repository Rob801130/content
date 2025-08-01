---
title: HTML attribute reference
short-title: Attributes
slug: Web/HTML/Reference/Attributes
page-type: landing-page
sidebar: htmlsidebar
---

Elements in HTML have **attributes**; these are additional values that configure the elements or adjust their behavior in various ways to meet the criteria the users want.

## Attribute list

<table class="standard-table">
  <thead>
    <tr>
      <th>Attribute Name</th>
      <th>Elements</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Attributes/accept">accept</a></code>
      </td>
      <td>
        {{ HTMLElement("form") }}, {{ HTMLElement("input") }}
      </td>
      <td>List of types the server accepts, typically a file type.</td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Elements/form#accept-charset">accept-charset</a></code>
      </td>
      <td>{{ HTMLElement("form") }}</td>
      <td>The character set, which if provided must be <code>"UTF-8"</code>.</td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Global_attributes/accesskey">accesskey</a></code>
      </td>
      <td>
        <a href="/en-US/docs/Web/HTML/Reference/Global_attributes">Global attribute</a>
      </td>
      <td>Keyboard shortcut to activate or add focus to the element.</td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Elements/form#action">action</a></code>
      </td>
      <td>{{ HTMLElement("form") }}</td>
      <td>
        The URI of a program that processes the information submitted via the
        form.
      </td>
    </tr>
    <tr>
      <td>
        <code>align</code> {{deprecated_inline}}
      </td>
      <td>
        {{ HTMLElement("caption") }}, {{ HTMLElement("col") }},
        {{ HTMLElement("colgroup") }},
        {{ HTMLElement("hr") }}, {{ HTMLElement("iframe") }},
        {{ HTMLElement("img") }}, {{ HTMLElement("table") }},
        {{ HTMLElement("tbody") }}, {{ HTMLElement("td") }},
        {{ HTMLElement("tfoot") }}, {{ HTMLElement("th") }},
        {{ HTMLElement("thead") }}, {{ HTMLElement("tr") }}
      </td>
      <td>Specifies the horizontal alignment of the element.</td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Elements/iframe#allow">allow</a></code>
      </td>
      <td>{{ HTMLElement("iframe") }}</td>
      <td>Specifies a feature-policy for the iframe.</td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Attributes/alt">alt</a></code>
      </td>
      <td>
        {{ HTMLElement("area") }},
        {{ HTMLElement("img") }}, {{ HTMLElement("input") }}
      </td>
      <td>Alternative text in case an image can't be displayed.</td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Elements/link#as">as</a></code>
      </td>
      <td>
        {{ HTMLElement("link") }}
      </td>
      <td>Specifies the type of content being loaded by the link.</td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Elements/script#async">async</a></code>
      </td>
      <td>{{ HTMLElement("script") }}</td>
      <td>Executes the script asynchronously.</td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Global_attributes/autocapitalize">autocapitalize</a></code>
      </td>
      <td>
        <a href="/en-US/docs/Web/HTML/Reference/Global_attributes">Global attribute</a>
      </td>
      <td>
        Sets whether input is automatically capitalized when entered by user
      </td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Attributes/autocomplete">autocomplete</a></code>
      </td>
      <td>
        {{ HTMLElement("form") }}, {{ HTMLElement("input") }},
        {{ HTMLElement("select") }},
        {{ HTMLElement("textarea") }}
      </td>
      <td>
        Indicates whether controls in this form can by default have their values
        automatically completed by the browser.
      </td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Attributes/autoplay">autoplay</a></code>
      </td>
      <td>
        {{ HTMLElement("audio") }},
        {{ HTMLElement("video") }}
      </td>
      <td>The audio or video should play as soon as possible.</td>
    </tr>
    <tr>
      <td><code>background</code></td>
      <td>
        {{ HTMLElement("body") }}, {{ HTMLElement("table") }},
        {{ HTMLElement("td") }}, {{ HTMLElement("th") }}
      </td>
      <td>
        Specifies the URL of an image file.
        <div class="note notecard">
          <p>
            <strong>Note:</strong> Although browsers and email clients may still
            support this attribute, it is obsolete. Use CSS
            {{ Cssxref("background-image") }} instead.
          </p>
        </div>
      </td>
    </tr>
    <tr>
      <td><code>bgcolor</code></td>
      <td>
        {{ HTMLElement("body") }}, {{ HTMLElement("col") }},
        {{ HTMLElement("colgroup") }},
        {{ HTMLElement("marquee") }},
        {{ HTMLElement("table") }},
        {{ HTMLElement("tbody") }},
        {{ HTMLElement("tfoot") }}, {{ HTMLElement("td") }},
        {{ HTMLElement("th") }}, {{ HTMLElement("tr") }}
      </td>
      <td>
        <p>Background color of the element.</p>
        <div class="note notecard">
          <p>
            <strong>Note:</strong> This is a legacy attribute. Please use the
            CSS {{ Cssxref("background-color") }} property instead.
          </p>
        </div>
      </td>
    </tr>
    <tr>
      <td><code>border</code></td>
      <td>
        {{ HTMLElement("img") }}, {{ HTMLElement("object") }},
        {{ HTMLElement("table") }}
      </td>
      <td>
        <p>The border width.</p>
        <div class="note notecard">
          <p>
            <strong>Note:</strong> This is a legacy attribute. Please use the
            CSS {{ Cssxref("border") }} property instead.
          </p>
        </div>
      </td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Attributes/capture">capture</a></code>
      </td>
      <td>{{ HTMLElement("input") }}</td>
      <td>
        From the <a href="https://w3c.github.io/html-media-capture/#the-capture-attribute">Media Capture specification</a>,
        specifies a new file can be captured.
      </td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Elements/meta#charset">charset</a></code>
      </td>
      <td>
        {{ HTMLElement("meta") }}
      </td>
      <td>Declares the character encoding of the page or script.</td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Elements/input#checked">checked</a></code>
      </td>
      <td>
        {{ HTMLElement("input") }}
      </td>
      <td>Indicates whether the element should be checked on page load.</td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Attributes/cite">cite</a></code>
      </td>
      <td>
        {{ HTMLElement("blockquote") }},
        {{ HTMLElement("del") }}, {{ HTMLElement("ins") }},
        {{ HTMLElement("q") }}
      </td>
      <td>Contains a URI which points to the source of the quote or change.</td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Global_attributes/class">class</a></code>
      </td>
      <td>
        <a href="/en-US/docs/Web/HTML/Reference/Global_attributes">Global attribute</a>
      </td>
      <td>Often used with CSS to style elements with common properties.</td>
    </tr>
    <tr>
      <td><code>color</code></td>
      <td>
        {{ HTMLElement("font") }}, {{ HTMLElement("hr") }}
      </td>
      <td>
        <p>
          This attribute sets the text color using either a named color or a
          color specified in the hexadecimal #RRGGBB format.
        </p>
        <div class="note notecard">
          <p>
            <strong>Note:</strong> This is a legacy attribute. Please use the
            CSS {{ Cssxref("color") }} property instead.
          </p>
        </div>
      </td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Elements/textarea#cols">cols</a></code>
      </td>
      <td>{{ HTMLElement("textarea") }}</td>
      <td>Defines the number of columns in a textarea.</td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Attributes/colspan">colspan</a></code>
      </td>
      <td>
        {{ HTMLElement("td") }}, {{ HTMLElement("th") }}
      </td>
      <td>
        The colspan attribute defines the number of columns a cell should span.
      </td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Attributes/content">content</a></code>
      </td>
      <td>{{ HTMLElement("meta") }}</td>
      <td>
        A value associated with <code>http-equiv</code> or
        <code>name</code> depending on the context.
      </td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Global_attributes/contenteditable">contenteditable</a></code>
      </td>
      <td>
        <a href="/en-US/docs/Web/HTML/Reference/Global_attributes">Global attribute</a>
      </td>
      <td>Indicates whether the element's content is editable.</td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Attributes/controls">controls</a></code>
      </td>
      <td>
        {{ HTMLElement("audio") }},
        {{ HTMLElement("video") }}
      </td>
      <td>
        Indicates whether the browser should show playback controls to the user.
      </td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Elements/area#coords">coords</a></code>
      </td>
      <td>{{ HTMLElement("area") }}</td>
      <td>
        A set of values specifying the coordinates of the hot-spot region.
      </td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Attributes/crossorigin">crossorigin</a></code>
      </td>
      <td>
        {{ HTMLElement("audio") }}, {{ HTMLElement("img") }},
        {{ HTMLElement("link") }}, {{ HTMLElement("script") }},
        {{ HTMLElement("video") }}
      </td>
      <td>How the element handles cross-origin requests</td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/API/HTMLIFrameElement/csp">csp</a></code>
        {{experimental_inline}}
      </td>
      <td>{{ HTMLElement("iframe") }}</td>
      <td>
        Specifies the Content Security Policy that an embedded document must
        agree to enforce upon itself.
      </td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Elements/object#data">data</a></code>
      </td>
      <td>{{ HTMLElement("object") }}</td>
      <td>Specifies the URL of the resource.</td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Global_attributes/data-*">data-*</a></code>
      </td>
      <td>
        <a href="/en-US/docs/Web/HTML/Reference/Global_attributes">Global attribute</a>
      </td>
      <td>Lets you attach custom attributes to an HTML element.</td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Attributes/datetime">datetime</a></code>
      </td>
      <td>
        {{ HTMLElement("del") }}, {{ HTMLElement("ins") }},
        {{ HTMLElement("time") }}
      </td>
      <td>Indicates the date and time associated with the element.</td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Elements/img#decoding">decoding</a></code>
      </td>
      <td>{{ HTMLElement("img") }}</td>
      <td>Indicates the preferred method to decode the image.</td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Elements/track#default">default</a></code>
      </td>
      <td>{{ HTMLElement("track") }}</td>
      <td>
        Indicates that the track should be enabled unless the user's preferences
        indicate something different.
      </td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Elements/script#defer">defer</a></code>
      </td>
      <td>{{ HTMLElement("script") }}</td>
      <td>
        Indicates that the script should be executed after the page has been
        parsed.
      </td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Global_attributes/dir">dir</a></code>
      </td>
      <td>
        <a href="/en-US/docs/Web/HTML/Reference/Global_attributes">Global attribute</a>
      </td>
      <td>
        Defines the text direction. Allowed values are ltr (Left-To-Right) or
        rtl (Right-To-Left)
      </td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Attributes/dirname">dirname</a></code>
      </td>
      <td>
        {{ HTMLElement("input") }},
        {{ HTMLElement("textarea") }}
      </td>
      <td></td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Attributes/disabled">disabled</a></code>
      </td>
      <td>
        {{ HTMLElement("button") }},
        {{ HTMLElement("fieldset") }},
        {{ HTMLElement("input") }},
        {{ HTMLElement("optgroup") }},
        {{ HTMLElement("option") }},
        {{ HTMLElement("select") }},
        {{ HTMLElement("textarea") }}
      </td>
      <td>Indicates whether the user can interact with the element.</td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Attributes/download">download</a></code>
      </td>
      <td>{{ HTMLElement("a") }}, {{ HTMLElement("area") }}</td>
      <td>
        Indicates that the hyperlink is to be used for downloading a resource.
      </td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Global_attributes/draggable">draggable</a></code>
      </td>
      <td>
        <a href="/en-US/docs/Web/HTML/Reference/Global_attributes">Global attribute</a>
      </td>
      <td>Defines whether the element can be dragged.</td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Elements/form#enctype">enctype</a></code>
      </td>
      <td>{{ HTMLElement("form") }}</td>
      <td>
        Defines the content type of the form data when the
        <code>method</code> is POST.
      </td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Global_attributes/enterkeyhint">enterkeyhint</a></code>
      </td>
      <td>
        {{ HTMLElement("textarea") }},
        <a href="/en-US/docs/Web/HTML/Reference/Global_attributes/contenteditable"><code>contenteditable</code></a>
      </td>
      <td>
        The <a href="https://html.spec.whatwg.org/multipage/interaction.html#input-modalities:-the-enterkeyhint-attribute"><code>enterkeyhint</code></a>
        specifies what action label (or icon) to present for the enter key on
        virtual keyboards. The attribute can be used with form controls (such as
        the value of <code>textarea</code> elements), or in elements in an
        editing host (e.g., using <code>contenteditable</code> attribute).
      </td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Attributes/elementtiming">elementtiming</a></code>
      </td>
      <td>
        {{htmlelement("img")}},
        {{SVGElement("image")}} elements inside an {{SVGElement("svg")}},
        poster images of {{htmlelement("video")}} elements,
        elements which have a {{cssxref("background-image")}},
        and elements containing text nodes, such as a {{htmlelement("p")}}
      </td>
      <td>
        Indicates that an element is flagged for tracking by {{domxref("PerformanceObserver")}} objects using the <code>"element"</code> type. For more details, see the {{domxref("PerformanceElementTiming")}} interface.
      </td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Attributes/for">for</a></code>
      </td>
      <td>
        {{ HTMLElement("label") }},
        {{ HTMLElement("output") }}
      </td>
      <td>Describes elements which belongs to this one.</td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Attributes/form">form</a></code>
      </td>
      <td>
        {{ HTMLElement("button") }},
        {{ HTMLElement("fieldset") }},
        {{ HTMLElement("input") }},
        {{ HTMLElement("label") }},
        {{ HTMLElement("meter") }},
        {{ HTMLElement("object") }},
        {{ HTMLElement("output") }},
        {{ HTMLElement("progress") }},
        {{ HTMLElement("select") }},
        {{ HTMLElement("textarea") }}
      </td>
      <td>Indicates the form that is the owner of the element.</td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Attributes/formaction">formaction</a></code>
      </td>
      <td>
        {{ HTMLElement("input") }},
        {{ HTMLElement("button") }}
      </td>
      <td>
        Indicates the action of the element, overriding the action defined in
        the {{ HTMLElement("form") }}.
      </td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Attributes/formenctype">formenctype</a></code>
      </td>
      <td>
        {{ HTMLElement("button") }},
        {{ HTMLElement("input") }}
      </td>
      <td>
        If the button/input is a {{Glossary("submit button")}} (e.g., <code>type="submit"</code>),
        this attribute sets the encoding type to use during form submission. If
        this attribute is specified, it overrides the
        <code>enctype</code> attribute of the button's
        <a href="/en-US/docs/Web/HTML/Reference/Elements/form">form</a> owner.
      </td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Attributes/formmethod">formmethod</a></code>
      </td>
      <td>
        {{ HTMLElement("button") }},
        {{ HTMLElement("input") }}
      </td>
      <td>
        If the button/input is a {{Glossary("submit button")}} (e.g., <code>type="submit"</code>),
        this attribute sets the submission method to use during form submission
        (<code>GET</code>, <code>POST</code>, etc.). If this attribute is
        specified, it overrides the <code>method</code> attribute of the
        button's <a href="/en-US/docs/Web/HTML/Reference/Elements/form">form</a> owner.
      </td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Attributes/formnovalidate">formnovalidate</a></code>
      </td>
      <td>
        {{ HTMLElement("button") }},
        {{ HTMLElement("input") }}
      </td>
      <td>
        If the button/input is a {{Glossary("submit button")}} (e.g., <code>type="submit"</code>),
        this boolean attribute specifies that the form is not to be validated
        when it is submitted. If this attribute is specified, it overrides the
        <code>novalidate</code> attribute of the button's
        <a href="/en-US/docs/Web/HTML/Reference/Elements/form">form</a> owner.
      </td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Attributes/formtarget">formtarget</a></code>
      </td>
      <td>
        {{ HTMLElement("button") }},
        {{ HTMLElement("input") }}
      </td>
      <td>
        If the button/input is a {{Glossary("submit button")}} (e.g., <code>type="submit"</code>),
        this attribute specifies the browsing context (for example, tab, window,
        or inline frame) in which to display the response that is received after
        submitting the form. If this attribute is specified, it overrides the
        <code>target</code> attribute of the button's
        <a href="/en-US/docs/Web/HTML/Reference/Elements/form">form</a> owner.
      </td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Attributes/headers">headers</a></code>
      </td>
      <td>
        {{ HTMLElement("td") }}, {{ HTMLElement("th") }}
      </td>
      <td>
        IDs of the <code>&#x3C;th></code> elements which applies to this
        element.
      </td>
    </tr>
    <tr>
      <td><code>height</code></td>
      <td>
        {{ HTMLElement("canvas") }},
        {{ HTMLElement("embed") }},
        {{ HTMLElement("iframe") }}, {{ HTMLElement("img") }},
        {{ HTMLElement("input") }},
        {{ HTMLElement("object") }},
        {{ HTMLElement("video") }}
      </td>
      <td>
        <p>
          Specifies the height of elements listed here. For all other elements,
          use the CSS {{cssxref("height")}} property.
        </p>
        <div class="note notecard">
          <p>
            <strong>Note:</strong> In some instances, such as
            {{ HTMLElement("div") }}, this is a legacy attribute, in
            which case the CSS {{ Cssxref("height") }} property should
            be used instead.
          </p>
        </div>
      </td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Global_attributes/hidden">hidden</a></code>
      </td>
      <td>
        <a href="/en-US/docs/Web/HTML/Reference/Global_attributes">Global attribute</a>
      </td>
      <td>
        Prevents rendering of given element, while keeping child elements, e.g.
        script elements, active.
      </td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Elements/meter#high">high</a></code>
      </td>
      <td>{{ HTMLElement("meter") }}</td>
      <td>Indicates the lower bound of the upper range.</td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Attributes/href">href</a></code>
      </td>
      <td>
        {{ HTMLElement("a") }}, {{ HTMLElement("area") }},
        {{ HTMLElement("base") }}, {{ HTMLElement("link") }}
      </td>
      <td>The URL of a linked resource.</td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Attributes/hreflang">hreflang</a></code>
      </td>
      <td>
        {{ HTMLElement("a") }}, {{ HTMLElement("link") }}
      </td>
      <td>Specifies the language of the linked resource.</td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Elements/meta/http-equiv">http-equiv</a></code>
      </td>
      <td>{{ HTMLElement("meta") }}</td>
      <td>Defines a pragma directive.</td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Global_attributes/id">id</a></code>
      </td>
      <td>
        <a href="/en-US/docs/Web/HTML/Reference/Global_attributes">Global attribute</a>
      </td>
      <td>
        Often used with CSS to style a specific element. The value of this
        attribute must be unique.
      </td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/Security/Subresource_Integrity">integrity</a></code>
      </td>
      <td>
        {{ HTMLElement("link") }}, {{ HTMLElement("script") }}
      </td>
      <td>
        <p>
          Specifies a
          <a href="/en-US/docs/Web/Security/Subresource_Integrity">Subresource Integrity</a>
          value that allows browsers to verify what they fetch.
        </p>
      </td>
    </tr>
    <tr>
      <td>
        <a href="/en-US/docs/Web/HTML/Reference/Global_attributes/inputmode"><code>inputmode</code></a>
      </td>
      <td>
        {{ HTMLElement("textarea") }},
        <a href="/en-US/docs/Web/HTML/Reference/Global_attributes/contenteditable"><code>contenteditable</code></a>
      </td>
      <td>
        Provides a hint as to the type of data that might be entered by the user
        while editing the element or its contents. The attribute can be used
        with form controls (such as the value of
        <code>textarea</code> elements), or in elements in an editing host
        (e.g., using <code>contenteditable</code> attribute).
      </td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Elements/img#ismap">ismap</a></code>
      </td>
      <td>{{ HTMLElement("img") }}</td>
      <td>Indicates that the image is part of a server-side image map.</td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Global_attributes/itemprop">itemprop</a></code>
      </td>
      <td>
        <a href="/en-US/docs/Web/HTML/Reference/Global_attributes">Global attribute</a>
      </td>
      <td></td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Elements/track#kind">kind</a></code>
      </td>
      <td>{{ HTMLElement("track") }}</td>
      <td>Specifies the kind of text track.</td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Attributes/label">label</a></code>
      </td>
      <td>
        {{ HTMLElement("optgroup") }},
        {{ HTMLElement("option") }},
        {{ HTMLElement("track") }}
      </td>
      <td>Specifies a user-readable title of the element.</td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Global_attributes/lang">lang</a></code>
      </td>
      <td>
        <a href="/en-US/docs/Web/HTML/Reference/Global_attributes">Global attribute</a>
      </td>
      <td>Defines the language used in the element.</td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Elements/script#language">language</a></code>
        {{deprecated_inline}}
      </td>
      <td>{{ HTMLElement("script") }}</td>
      <td>Defines the script language used in the element.</td>
    </tr>
    <tr>
      <td><code>loading</code></td>
      <td>
        {{ HTMLElement("img") }}, {{ HTMLElement("iframe") }}
      </td>
      <td>
        Indicates if the element should be loaded lazily
        (<code>loading="lazy"</code>) or loaded immediately
        (<code>loading="eager"</code>).
      </td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Elements/input#list">list</a></code>
      </td>
      <td>{{ HTMLElement("input") }}</td>
      <td>Identifies a list of pre-defined options to suggest to the user.</td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Attributes/loop">loop</a></code>
      </td>
      <td>
        {{ HTMLElement("audio") }},
        {{ HTMLElement("marquee") }},
        {{ HTMLElement("video") }}
      </td>
      <td>
        Indicates whether the media should start playing from the start when
        it's finished.
      </td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Elements/meter#low">low</a></code>
      </td>
      <td>{{ HTMLElement("meter") }}</td>
      <td>Indicates the upper bound of the lower range.</td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Attributes/max">max</a></code>
      </td>
      <td>
        {{ HTMLElement("input") }},
        {{ HTMLElement("meter") }},
        {{ HTMLElement("progress") }}
      </td>
      <td>Indicates the maximum value allowed.</td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Attributes/maxlength">maxlength</a></code>
      </td>
      <td>
        {{ HTMLElement("input") }},
        {{ HTMLElement("textarea") }}
      </td>
      <td>Defines the maximum number of characters allowed in the element.</td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Attributes/minlength">minlength</a></code>
      </td>
      <td>
        {{ HTMLElement("input") }},
        {{ HTMLElement("textarea") }}
      </td>
      <td>Defines the minimum number of characters allowed in the element.</td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Attributes/media">media</a></code>
      </td>
      <td>
        {{ HTMLElement("a") }}, {{ HTMLElement("area") }},
        {{ HTMLElement("link") }}, {{ HTMLElement("source") }},
        {{ HTMLElement("style") }}
      </td>
      <td>
        Specifies a hint of the media for which the linked resource was
        designed.
      </td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Elements/form#method">method</a></code>
      </td>
      <td>{{ HTMLElement("form") }}</td>
      <td>
        Defines which <a href="/en-US/docs/Web/HTTP">HTTP</a> method to use when
        submitting the form. Can be <code>GET</code> (default) or
        <code>POST</code>.
      </td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Attributes/min">min</a></code>
      </td>
      <td>
        {{ HTMLElement("input") }},
        {{ HTMLElement("meter") }}
      </td>
      <td>Indicates the minimum value allowed.</td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Attributes/multiple">multiple</a></code>
      </td>
      <td>
        {{ HTMLElement("input") }},
        {{ HTMLElement("select") }}
      </td>
      <td>
        Indicates whether multiple values can be entered in an input of the type
        <code>email</code> or <code>file</code>.
      </td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Attributes/muted">muted</a></code>
      </td>
      <td>
        {{ HTMLElement("audio") }},
        {{ HTMLElement("video") }}
      </td>
      <td>
        Indicates whether the audio will be initially silenced on page load.
      </td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Attributes/name">name</a></code>
      </td>
      <td>
        {{ HTMLElement("button") }}, {{ HTMLElement("form") }},
        {{ HTMLElement("fieldset") }},
        {{ HTMLElement("iframe") }},
        {{ HTMLElement("input") }},
        {{ HTMLElement("object") }},
        {{ HTMLElement("output") }},
        {{ HTMLElement("select") }},
        {{ HTMLElement("textarea") }},
        {{ HTMLElement("map") }}, {{ HTMLElement("meta") }},
        {{ HTMLElement("param") }}
      </td>
      <td>
        Name of the element. For example used by the server to identify the
        fields in form submits.
      </td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Elements/form#novalidate">novalidate</a></code>
      </td>
      <td>{{ HTMLElement("form") }}</td>
      <td>
        This attribute indicates that the form shouldn't be validated when
        submitted.
      </td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Attributes/open">open</a></code>
      </td>
      <td>
        {{ HTMLElement("details") }},
        {{ HTMLElement("dialog") }}
      </td>
      <td>
        Indicates whether the contents are currently visible (in the case of
        a <code>&#x3C;details></code> element) or whether the dialog is active
        and can be interacted with (in the case of a
        <code>&#x3C;dialog></code> element).
      </td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Elements/meter#optimum">optimum</a></code>
      </td>
      <td>{{ HTMLElement("meter") }}</td>
      <td>Indicates the optimal numeric value.</td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Attributes/pattern">pattern</a></code>
      </td>
      <td>{{ HTMLElement("input") }}</td>
      <td>
        Defines a regular expression which the element's value will be validated
        against.
      </td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Elements/a#ping">ping</a></code>
      </td>
      <td>{{ HTMLElement("a") }}, {{ HTMLElement("area") }}</td>
      <td>
        The <code>ping</code> attribute specifies a space-separated list of URLs
        to be notified if a user follows the hyperlink.
      </td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Attributes/placeholder">placeholder</a></code>
      </td>
      <td>
        {{ HTMLElement("input") }},
        {{ HTMLElement("textarea") }}
      </td>
      <td>Provides a hint to the user of what can be entered in the field.</td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Elements/video#playsinline">playsinline</a></code>
      </td>
      <td>
        {{ HTMLElement("video") }}
      </td>
      <td>A Boolean attribute indicating that the video is to be played "inline"; that is, within the element's playback area. Note that the absence of this attribute does not imply that the video will always be played in fullscreen.</td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Elements/video#poster">poster</a></code>
      </td>
      <td>{{ HTMLElement("video") }}</td>
      <td>
        A URL indicating a poster frame to show until the user plays or seeks.
      </td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Attributes/preload">preload</a></code>
      </td>
      <td>
        {{ HTMLElement("audio") }},
        {{ HTMLElement("video") }}
      </td>
      <td>
        Indicates whether the whole resource, parts of it or nothing should be
        preloaded.
      </td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Attributes/readonly">readonly</a></code>
      </td>
      <td>
        {{ HTMLElement("input") }},
        {{ HTMLElement("textarea") }}
      </td>
      <td>Indicates whether the element can be edited.</td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Attributes/referralpolicy">referrerpolicy</a></code>
      </td>
      <td>
        {{ HTMLElement("a") }}, {{ HTMLElement("area") }},
        {{ HTMLElement("iframe") }}, {{ HTMLElement("img") }},
        {{ HTMLElement("link") }}, {{ HTMLElement("script") }}
      </td>
      <td>Specifies which referrer is sent when fetching the resource.</td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Attributes/rel">rel</a></code>
      </td>
      <td>
        {{ HTMLElement("a") }}, {{ HTMLElement("area") }},
        {{ HTMLElement("link") }}
      </td>
      <td>
        Specifies the relationship of the target object to the link object.
      </td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Attributes/required">required</a></code>
      </td>
      <td>
        {{ HTMLElement("input") }},
        {{ HTMLElement("select") }},
        {{ HTMLElement("textarea") }}
      </td>
      <td>Indicates whether this element is required to fill out or not.</td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Elements/ol#reversed">reversed</a></code>
      </td>
      <td>{{ HTMLElement("ol") }}</td>
      <td>
        Indicates whether the list should be displayed in a descending order
        instead of an ascending order.
      </td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/Accessibility/ARIA/Reference/Roles">role</a></code>
      </td>
      <td><a href="/en-US/docs/Web/HTML/Reference/Global_attributes">Global attribute</a></td>
      <td>Defines an explicit role for an element for use by assistive technologies.</td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Elements/textarea#rows">rows</a></code>
      </td>
      <td>{{ HTMLElement("textarea") }}</td>
      <td>Defines the number of rows in a text area.</td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Attributes/rowspan">rowspan</a></code>
      </td>
      <td>
        {{ HTMLElement("td") }}, {{ HTMLElement("th") }}
      </td>
      <td>Defines the number of rows a table cell should span over.</td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Elements/iframe#sandbox">sandbox</a></code>
      </td>
      <td>{{ HTMLElement("iframe") }}</td>
      <td>
        Stops a document loaded in an iframe from using certain features (such
        as submitting forms or opening new windows).
      </td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Elements/th#scope">scope</a></code>
      </td>
      <td>{{ HTMLElement("th") }}</td>
      <td>
        Defines the cells that the header test (defined in the
        <code>th</code> element) relates to.
      </td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Elements/option#selected">selected</a></code>
      </td>
      <td>{{ HTMLElement("option") }}</td>
      <td>Defines a value which will be selected on page load.</td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Attributes/shape">shape</a></code>
      </td>
      <td>{{ HTMLElement("a") }}, {{ HTMLElement("area") }}</td>
      <td></td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Attributes/size">size</a></code>
      </td>
      <td>
        {{ HTMLElement("input") }},
        {{ HTMLElement("select") }}
      </td>
      <td>
        Defines the width of the element (in pixels). If the element's
        <code>type</code> attribute is <code>text</code> or
        <code>password</code> then it's the number of characters.
      </td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Attributes/sizes">sizes</a></code>
      </td>
      <td>
        {{ HTMLElement("link") }}, {{ HTMLElement("img") }},
        {{ HTMLElement("source") }}
      </td>
      <td></td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Global_attributes/slot">slot</a></code>
      </td>
      <td>
        <a href="/en-US/docs/Web/HTML/Reference/Global_attributes">Global attribute</a>
      </td>
      <td>Assigns a slot in a shadow DOM shadow tree to an element.</td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Attributes/span">span</a></code>
      </td>
      <td>
        {{ HTMLElement("col") }},
        {{ HTMLElement("colgroup") }}
      </td>
      <td></td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Global_attributes/spellcheck">spellcheck</a></code>
      </td>
      <td>
        <a href="/en-US/docs/Web/HTML/Reference/Global_attributes">Global attribute</a>
      </td>
      <td>Indicates whether spell checking is allowed for the element.</td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Attributes/src">src</a></code>
      </td>
      <td>
        {{ HTMLElement("audio") }},
        {{ HTMLElement("embed") }},
        {{ HTMLElement("iframe") }}, {{ HTMLElement("img") }},
        {{ HTMLElement("input") }},
        {{ HTMLElement("script") }},
        {{ HTMLElement("source") }},
        {{ HTMLElement("track") }},
        {{ HTMLElement("video") }}
      </td>
      <td>The URL of the embeddable content.</td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Elements/iframe#srcdoc">srcdoc</a></code>
      </td>
      <td>{{ HTMLElement("iframe") }}</td>
      <td></td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Elements/track#srclang">srclang</a></code>
      </td>
      <td>{{ HTMLElement("track") }}</td>
      <td></td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Attributes/srcset">srcset</a></code>
      </td>
      <td>
        {{ HTMLElement("img") }}, {{ HTMLElement("source") }}
      </td>
      <td>One or more responsive image candidates.</td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Elements/ol#start">start</a></code>
      </td>
      <td>{{ HTMLElement("ol") }}</td>
      <td>Defines the first number if other than 1.</td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Attributes/step">step</a></code>
      </td>
      <td>{{ HTMLElement("input") }}</td>
      <td></td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Global_attributes/style">style</a></code>
      </td>
      <td>
        <a href="/en-US/docs/Web/HTML/Reference/Global_attributes">Global attribute</a>
      </td>
      <td>Defines CSS styles which will override styles previously set.</td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Elements/table#summary">summary</a></code>
        {{deprecated_inline}}
      </td>
      <td>{{ HTMLElement("table") }}</td>
      <td></td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Global_attributes/tabindex">tabindex</a></code>
      </td>
      <td>
        <a href="/en-US/docs/Web/HTML/Reference/Global_attributes">Global attribute</a>
      </td>
      <td>
        Overrides the browser's default tab order and follows the one specified
        instead.
      </td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Attributes/target">target</a></code>
      </td>
      <td>
        {{ HTMLElement("a") }}, {{ HTMLElement("area") }},
        {{ HTMLElement("base") }}, {{ HTMLElement("form") }}
      </td>
      <td>
        Specifies where to open the linked document (in the case of an
        <code>&#x3C;a></code> element) or where to display the response received
        (in the case of a <code>&#x3C;form></code> element)
      </td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Global_attributes/title">title</a></code>
      </td>
      <td>
        <a href="/en-US/docs/Web/HTML/Reference/Global_attributes">Global attribute</a>
      </td>
      <td>Text to be displayed in a tooltip when hovering over the element.</td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Global_attributes/translate">translate</a></code>
      </td>
      <td>
        <a href="/en-US/docs/Web/HTML/Reference/Global_attributes">Global attribute</a>
      </td>
      <td>
        Specify whether an element's attribute values and the values of its
        <code><a href="https://dom.spec.whatwg.org/#text">Text</a></code> node
        children are to be translated when the page is localized, or whether to
        leave them unchanged.
      </td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Attributes/type">type</a></code>
      </td>
      <td>
        {{ HTMLElement("button") }},
        {{ HTMLElement("input") }},
        {{ HTMLElement("embed") }},
        {{ HTMLElement("object") }},
        {{ HTMLElement("ol") }},
        {{ HTMLElement("script") }},
        {{ HTMLElement("source") }},
        {{ HTMLElement("style") }}, {{ HTMLElement("menu") }},
        {{ HTMLElement("link") }}
      </td>
      <td>Defines the type of the element.</td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Attributes/usemap">usemap</a></code>
      </td>
      <td>
        {{ HTMLElement("img") }}, {{ HTMLElement("input") }},
        {{ HTMLElement("object") }}
      </td>
      <td></td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Attributes/value">value</a></code>
      </td>
      <td>
        {{ HTMLElement("button") }}, {{ HTMLElement("data") }},
        {{ HTMLElement("input") }}, {{ HTMLElement("li") }},
        {{ HTMLElement("meter") }},
        {{ HTMLElement("option") }},
        {{ HTMLElement("progress") }},
        {{ HTMLElement("param") }}
      </td>
      <td>
        Defines a default value which will be displayed in the element on page
        load.
      </td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Attributes/width">width</a></code>
      </td>
      <td>
        {{ HTMLElement("canvas") }},
        {{ HTMLElement("embed") }},
        {{ HTMLElement("iframe") }}, {{ HTMLElement("img") }},
        {{ HTMLElement("input") }},
        {{ HTMLElement("object") }},
        {{ HTMLElement("video") }}
      </td>
      <td>
        <p>
          For the elements listed here, this establishes the element's width.
        </p>
        <div class="note notecard">
          <p>
            <strong>Note:</strong> For all other instances, such as
            {{ HTMLElement("div") }}, this is a legacy attribute, in
            which case the CSS {{ Cssxref("width") }} property should be
            used instead.
          </p>
        </div>
      </td>
    </tr>
    <tr>
      <td>
        <code><a href="/en-US/docs/Web/HTML/Reference/Elements/textarea#wrap">wrap</a></code>
      </td>
      <td>{{ HTMLElement("textarea") }}</td>
      <td>Indicates whether the text should be wrapped.</td>
    </tr>
  </tbody>
</table>

## Content versus IDL attributes

In HTML, most attributes have two faces: the **content attribute** and the **IDL (Interface Definition Language) attribute**.

The content attribute is the attribute as you set it from the content (the HTML code) and you can set it or get it via {{domxref("element.setAttribute()")}} or {{domxref("element.getAttribute()")}}. The content attribute is always a string even when the expected value should be an integer. For example, to set an {{HTMLElement("input")}} element's `maxlength` to 42 using the content attribute, you have to call `setAttribute("maxlength", "42")` on that element.

The IDL attribute is also known as a JavaScript property. These are the attributes you can read or set using JavaScript properties like `element.foo`. The IDL attribute is always going to use (but might transform) the underlying content attribute to return a value when you get it and is going to save something in the content attribute when you set it. In other words, the IDL attributes, in essence, reflect the content attributes.

Most of the time, IDL attributes will return their values as they are really used. For example, the default `type` for {{HTMLElement("input")}} elements is "text", so if you set `input.type="foobar"`, the `<input>` element will be of type text (in the appearance and the behavior) but the "type" content attribute's value will be "foobar". However, the `type` IDL attribute will return the string "text".

IDL attributes are not always strings; for example, `input.maxlength` is a number (a signed long). When using IDL attributes, you read or set values of the desired type, so `input.maxlength` is always going to return a number and when you set `input.maxlength`, it wants a number. If you pass another type, it is automatically converted to a number as specified by the standard JavaScript rules for type conversion.

IDL attributes can [reflect other types](https://html.spec.whatwg.org/multipage/urls-and-fetching.html) such as unsigned long, URLs, booleans, etc. Unfortunately, there are no clear rules and the way IDL attributes behave in conjunction with their corresponding content attributes depends on the attribute. Most of the time, it will follow [the rules laid out in the specification](https://html.spec.whatwg.org/multipage/urls-and-fetching.html), but sometimes it doesn't. HTML specifications try to make this as developer-friendly as possible, but for various reasons (mostly historical), some attributes behave oddly (`select.size`, for example) and you should read the specifications to understand how exactly they behave.

## Boolean Attributes

Some content attributes (e.g., `required`, `readonly`, `disabled`) are called [boolean attributes](https://html.spec.whatwg.org/multipage/common-microsyntaxes.html#boolean-attributes). If a boolean attribute is present, its value is **true**, and if it's absent, its value is **false**.

HTML defines restrictions on the allowed values of boolean attributes: If the attribute is present, its value must either be the empty string (equivalently, the attribute may have an unassigned value), or a value that is an ASCII case-insensitive match for the attribute's canonical name, with no leading or trailing whitespace. The following examples are valid ways to mark up a boolean attribute:

```html-nolint
<div itemscope>This is valid HTML but invalid XML.</div>
<div itemscope=itemscope>This is also valid HTML but invalid XML.</div>
<div itemscope="">This is valid HTML and also valid XML.</div>
<div itemscope="itemscope">
  This is also valid HTML and XML, but perhaps a bit verbose.
</div>
```

To be clear, the values `"true"` and `"false"` are not allowed on boolean attributes. To represent a false value, the attribute has to be omitted altogether. This restriction clears up some common misunderstandings: With `checked="false"` for example, the element's `checked` attribute would be interpreted as **true** because the attribute is present.

## Event handler attributes

> [!WARNING]
> The use of event handler content attributes is discouraged. The mix of HTML and JavaScript often produces unmaintainable code, and the execution of event handler attributes may also be blocked by content security policies.

In addition to the attributes listed in the table above, global [event handlers](/en-US/docs/Web/API/Document_Object_Model/Events#using_onevent_properties) — such as [`onclick`](/en-US/docs/Web/API/Element/click_event) — can also be specified as [content attributes](#content_versus_idl_attributes) on all elements.

All event handler attributes accept a string. The string will be used to synthesize a [JavaScript function](/en-US/docs/Web/JavaScript/Reference/Functions) like `function name(/*args*/) {body}`, where `name` is the attribute's name, and `body` is the attribute's value. The handler receives the same parameters as its JavaScript event handler counterpart — most handlers receive only one `event` parameter, while `onerror` receives five: `event`, `source`, `lineno`, `colno`, `error`. This means you can, in general, use the `event` variable within the attribute.

```html
<div onclick="console.log(event)">Click me!</div>
<!-- The synthesized handler has a name; you can reference itself -->
<div onclick="console.log(onclick)">Click me!</div>
```

## See also

- [HTML elements](/en-US/docs/Web/HTML/Reference/Elements)
