# Tutorial 2

## Review Assignment

---

### [@charset - CSS: Cascading Style Sheets | MDN](https://developer.mozilla.org/en-US/docs/Web/CSS/@charset)

> @charset
The @charset CSS at-rule specifies the character encoding used in the style sheet. It must be the first element in the style sheet and not be preceded by any character; as it is not a nested statement, it cannot be used inside conditional group at-rules. If several @charset at-rules are defined, only the first one is used, and it cannot be used inside a style attribute on an HTML element or inside the \<style> element where the character set of the HTML page is relevant.

```css
@charset "utf-8";
```

---

### [@font-face - CSS: Cascading Style Sheets | MDN](https://developer.mozilla.org/en-US/docs/Web/CSS/@font-face)

> The @font-face CSS at-rule specifies a custom font with which to display text; the font can be loaded from either a remote server or a locally-installed font on the user's own computer.

#### Syntax

```css
@font-face {
  font-family: "Open Sans";
  src: url("/fonts/OpenSans-Regular-webfont.woff2") format("woff2"),
       url("/fonts/OpenSans-Regular-webfont.woff") format("woff");
}
```

---

### [background-color - CSS: Cascading Style Sheets | MDN](https://developer.mozilla.org/en-US/docs/Web/CSS/background-color)

> The background-color CSS property sets the background color of an element.

#### Syntax

```css
/* Keyword values */
background-color: red;
background-color: indigo;

/* Hexadecimal value */
background-color: #bbff00;    /* Fully opaque */
background-color: #bf0;       /* Fully opaque shorthand */
background-color: #11ffee00;  /* Fully transparent */
background-color: #1fe0;      /* Fully transparent shorthand  */
background-color: #11ffeeff;  /* Fully opaque */
background-color: #1fef;      /* Fully opaque shorthand  */

/* RGB value */
background-color: rgb(255, 255, 128);        /* Fully opaque */
background-color: rgba(117, 190, 218, 0.5);  /* 50% transparent */

/* HSL value */
background-color: hsl(50, 33%, 25%);         /* Fully opaque */
background-color: hsla(50, 33%, 25%, 0.75);  /* 75% opaque, i.e. 25% transparent */

/* Special keyword values */
background-color: currentcolor;
background-color: transparent;

/* Global values */
background-color: inherit;
background-color: initial;
background-color: revert;
background-color: unset;
```

---

### [color - CSS: Cascading Style Sheets | MDN](https://developer.mozilla.org/en-US/docs/Web/CSS/color)

> The color CSS property sets the foreground color value of an element's text and text decorations, and sets the \<currentcolor> value. currentcolor may be used as an indirect value on other properties and is the default for other color properties, such as border-color.
For an overview of using color in HTML, see Applying color to HTML elements using CSS.

#### Syntax

```css
/* Keyword values */
color: currentcolor;

/* <named-color> values */
color: red;
color: orange;
color: tan;
color: rebeccapurple;

/* <hex-color> values */
color: #090;
color: #009900;
color: #090a;
color: #009900aa;

/* <rgb()> values */
color: rgb(34, 12, 64, 0.6);
color: rgba(34, 12, 64, 0.6);
color: rgb(34 12 64 / 0.6);
color: rgba(34 12 64 / 0.3);
color: rgb(34.0 12 64 / 60%);
color: rgba(34.6 12 64 / 30%);

/* <hsl()> values */
color: hsl(30, 100%, 50%, 0.6);
color: hsla(30, 100%, 50%, 0.6);
color: hsl(30 100% 50% / 0.6);
color: hsla(30 100% 50% / 0.6);
color: hsl(30.0 100% 50% / 60%);
color: hsla(30.2 100% 50% / 60%);

/* Global values */
color: inherit;
color: initial;
color: revert;
color: unset;
```

---

### [font-family - CSS: Cascading Style Sheets | MDN](https://developer.mozilla.org/en-US/docs/Web/CSS/font-family)

> The font-family CSS property specifies a prioritized list of one or more font family names and/or generic family names for the selected element.
Values are separated by commas to indicate that they are alternatives. The browser will select the first font in the list that is installed or that can be downloaded using a @font-face at-rule.

It is often convenient to use the shorthand property font to set font-size and other font related properties all at once.

You should always include at least one generic family name in a font-family list, since there's no guarantee that any given font is available. This lets the browser select an acceptable fallback font when necessary.

The font-family property specifies a list of fonts, from highest priority to lowest. Font selection does not stop at the first font in the list that is on the user's system. Rather, font selection is done one character at a time, so that if an available font does not have a glyph for a needed character, the latter fonts are tried. When a font is only available in some styles, variants, or sizes, those properties may also influence which font family is chosen.

#### Syntax

```css
/* A font family name and a generic family name */
font-family: "Gill Sans Extrabold", sans-serif;
font-family: "Goudy Bookletter 1911", sans-serif;

/* A generic family name only */
font-family: serif;
font-family: sans-serif;
font-family: monospace;
font-family: cursive;
font-family: fantasy;
font-family: system-ui;
font-family: ui-serif;
font-family: ui-sans-serif;
font-family: ui-monospace;
font-family: ui-rounded;
font-family: emoji;
font-family: math;
font-family: fangsong;
```

---

### [font - CSS: Cascading Style Sheets | MDN](https://developer.mozilla.org/en-US/docs/Web/CSS/font)

> The font CSS shorthand property sets all the different properties of an element's font. Alternatively, it sets an element's font to a system font.

---

### [text-align - CSS: Cascading Style Sheets | MDN](https://developer.mozilla.org/en-US/docs/Web/CSS/text-align)

> The text-align CSS property sets the horizontal alignment of the content inside a block element or table-cell box. This means it works like vertical-align but in the horizontal direction.

#### Syntax

```css
/* Keyword values */
text-align: start;
text-align: end;
text-align: left;
text-align: right;
text-align: center;
text-align: justify;
text-align: justify-all;
text-align: match-parent;

/* Character-based alignment in a table column */
text-align: ".";
text-align: "." center;

/* Block alignment values (Non-standard syntax) */
text-align: -moz-center;
text-align: -webkit-center;
```

---

### [padding-left - CSS: Cascading Style Sheets | MDN](https://developer.mozilla.org/en-US/docs/Web/CSS/padding-left)

> The padding-left CSS property sets the width of the padding area to the left of an element.

An element's padding area is the space between its content and its border.

Note: The padding property can be used to set paddings on all four sides of an element with a single declaration.

#### Syntax

```css
/* <length> values */
padding-left: 0.5em;
padding-left: 0;
padding-left: 2cm;

/* <percentage> value */
padding-left: 10%;
```

---

### [font-weight - CSS: Cascading Style Sheets | MDN](https://developer.mozilla.org/en-US/docs/Web/CSS/font-weight)

> The font-weight CSS property sets the weight (or boldness) of the font. The weights available depend on the font-family that is currently set.

#### Syntax

```css
/* Keyword values */
font-weight: normal;
font-weight: bold;
```

---

### [letter-spacing - CSS: Cascading Style Sheets | MDN](https://developer.mozilla.org/en-US/docs/Web/CSS/letter-spacing)

> The letter-spacing CSS property sets the horizontal spacing behavior between text characters. This value is added to the natural spacing between characters while rendering the text. Positive values of letter-spacing causes characters to spread farther apart, while negative values of letter-spacing bring characters closer together.

#### Syntax

```css
/* Keyword value */
letter-spacing: normal;

/* <length> values */
letter-spacing: 0.3em;
letter-spacing: 3px;
letter-spacing: .3px;
```

---

### [quotes - CSS: Cascading Style Sheets | MDN](https://developer.mozilla.org/en-US/docs/Web/CSS/quotes)

> The quotes CSS property sets how the browser should render quotation marks that are added using the open-quotes or close-quotes values of the CSS content property.

#### Syntax

```css
/* Keyword value */
quotes: none;
quotes: auto;

/* <string> values */
quotes: "«" "»";           /* Set open-quote and close-quote to the French quotation marks */
quotes: "«" "»" "‹" "›";   /* Set two levels of quotation marks */
```

---

### [content - CSS: Cascading Style Sheets | MDN](https://developer.mozilla.org/en-US/docs/Web/CSS/content)

> The content CSS property replaces an element with a generated value. Objects inserted using the content property are anonymous replaced elements.

#### Syntax

```css
/* Keywords that cannot be combined with other values */
content: normal;
content: none;

/* <image> values */
content: url("http://www.example.com/test.png");
content: linear-gradient(#e66465, #9198e5);
content: image-set("image1x.png" 1x, "image2x.png" 2x);

/* alt text for generated content, added in the Level 3 specification */
content: url("http://www.example.com/test.png") / "This is the alt text";

/* <string> value */
content: "prefix";

/* <counter> values, optionally with <list-style-type> */
content: counter(chapter_counter);
content: counter(chapter_counter, upper-roman);
content: counters(section_counter, ".");
content: counters(section_counter, ".", decimal-leading-zero);

/* attr() value linked to the HTML attribute value */
content: attr(value string);

/* Language- and position-dependent keywords */
content: open-quote;
content: close-quote;
content: no-open-quote;
content: no-close-quote;
```

---

### [line-height - CSS: Cascading Style Sheets | MDN](https://developer.mozilla.org/en-US/docs/Web/CSS/line-height)

> The line-height CSS property sets the height of a line box. It's commonly used to set the distance between lines of text. On block-level elements, it specifies the minimum height of line boxes within the element. On non-replaced inline elements, it specifies the height that is used to calculate line box height.

#### Syntax

```css
/* Keyword value */
line-height: normal;

/* Unitless values: use this number multiplied
by the element's font size */
line-height: 3.5;

/* <length> values */
line-height: 3em;

/* <percentage> values */
line-height: 34%;
```
