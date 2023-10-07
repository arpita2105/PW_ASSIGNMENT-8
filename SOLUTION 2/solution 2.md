# SOLUTION

## **Absolute and Relative Positioning**
Absolute and relative positioning is a property in CSS that allows you to position an element.

## DIFFERENCE BETWEEN ABSOLUTE AND RELATIVE POSITIONING


### Relative Positioning
Relative positioning is a property in CSS that allows you to positions an element relative to its normal position in the document flow.

- You can use properties like `top`, `right`, `bottom`, and `left` with relative positioning to adjust the element's position relative to its normal flow position.
- Elements with relative positioning can affect the layout of other elements on the page. If they are moved, other elements may adjust their positions accordingly.
- However, unlike absolute positioning, elements with relative positioning are not taken out of the normal document flow. They still occupy space as if they were in their original position.

An element with `position: relative;` property is positioned relative to its normal position.

```css
div.relative {
  position: relative;
  left: 30px;
  border: 3px solid #73AD21;
}
```

### Absolute Positioning
Absolute positioning is a property in CSS that allows you to position an element on a web page or in a document relative to a parent element or the document itself.

- When an element is absolutely positioned, it is taken out of the normal document flow, and its position is determined based on its containing block (usually the nearest positioned ancestor or the document itself if there is none).
- The position of an element is defined using properties like top, right, bottom, and left, which specify how far the element should be offset from the edges of its containing block.
- Elements with absolute positioning are not affected by other elements, and they can overlap with other elements on the page.

An element with `position: absolute;` is positioned relative to the nearest positioned ancestor (instead of positioned relative to the viewport, like fixed).

-However; if an absolute positioned element has no positioned ancestors, it uses the document body, and moves along with page scrolling.

**Note:** Absolute positioned elements are removed from the normal flow, and can overlap elements.

```css
div.relative {
  position: relative;
  width: 400px;
  height: 200px;
  border: 3px solid #73AD21;
}

div.absolute {
  position: absolute;
  top: 80px;
  right: 0;
  width: 200px;
  height: 100px;
  border: 3px solid #73AD21;
}
```