---
title: Window.scrollTo()
slug: Web/API/Window/scrollTo
page-type: web-api-instance-method
tags:
  - API
  - CSSOM View
  - Method
  - NeedsMarkupWork
  - Reference
browser-compat: api.Window.scrollTo
---
{{APIRef}}

**`Window.scrollTo()`** scrolls to a particular set of
coordinates in the document.

## Syntax

```js
scrollTo(x-coord, y-coord)
scrollTo(options)
```

### Parameters

- `x-coord` is the pixel along the horizontal axis of the
  document that you want displayed in the upper left.
- `y-coord` is the pixel along the vertical axis of the document
  that you want displayed in the upper left.

\- or -

- `options`
  - : A dictionary containing the following parameters:
    - `top`
      - : (Optional) Specifies the number pixels from the top of Y axis to scroll the window or element.
    - `left`
      - : (Optional) Specifies the number of pixels from the top of the X axis to scroll the window or element.
    - `behavior`
      - : (Optional) Specifies whether the scrolling should animate smoothly (`smooth`), or happen instantly in a single jump (`auto`, the default value).

### Return value

None ({{jsxref("undefined")}}).

## Examples

```js
window.scrollTo(0, 1000);
```

Using `options`:

```js
window.scrollTo({
  top: 1000,
  left: 0,
  behavior: 'smooth'
});
```

## Notes

{{domxref("Window.scroll()")}} is effectively the same as this method. For relative
scrolling, see {{domxref("Window.scrollBy()")}}, {{domxref("Window.scrollByLines()")}},
and {{domxref("Window.scrollByPages()")}}.

For scrolling elements, see {{domxref("Element.scrollTop")}} and
{{domxref("Element.scrollLeft")}}.

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}
