# HTML & CSS Learning Journey 🚀

## 📅 Daily Log

| Day | Date         | Topic                                                 | Status |
| --- | ------------ | ----------------------------------------------------- | ------ |
| 01  | 10 June 2026 | CSS Priority — Inline, Internal, External, !important | ✅      |
| 02  | 11 June 2026 | CSS Box Model — Border, Padding, Margin, Box Sizing   | ✅      |
| 03  | 12 June 2026 | CSS Selectors & Pseudo Classes                        | ✅      |
| 04  | 13 June 2026 | Text & Font Properties                                | ✅      |

---

# 📖 Notes

## 📅 10 June 2026

### CSS Priority

Priority Order:

```text
!important
↓
Inline CSS
↓
Internal CSS
↓
External CSS
```

Example:

```html
<p style="color:red;">
  Hello
</p>
```

```css
p{
  color:blue;
}
```

Output:

```text
Red
```

### !important Override

```html
<p style="color:red;">
  Hello
</p>
```

```css
p{
  color:blue !important;
}
```

Output:

```text
Blue
```

### Important Notes

```text
!important > Inline > Internal > External
```

* Avoid excessive use of `!important`
* Makes debugging difficult
* Mostly used to force an override

---

## 📅 11 June 2026

### CSS Box Model

Browser Default:

```css
box-sizing:content-box;
```

Formula:

```text
Actual Width = Content + Padding + Border
```

Example:

```css
width:200px;
padding:20px;
border:10px solid;
```

Calculation:

```text
200 + 40 + 20 = 260px
```

---

### Border Box

```css
box-sizing:border-box;
```

Formula:

```text
Width = Content + Padding + Border
```

Example:

```css
width:200px;
padding:20px;
border:10px solid;
box-sizing:border-box;
```

Actual Width:

```text
200px
```

### Why Border Box Is Preferred

```text
Easier layout calculations
More predictable sizing
Used in almost every modern project
```

---

### Margin

Creates space outside the element.

```css
margin:auto;
margin-top:80px;
margin-bottom:100px;
```

Important:

```text
margin:auto works for horizontal centering
when element has a defined width
```

---

### Padding

Creates space inside the element.

```css
padding-top:20px;
padding-right:23px;
padding-bottom:52px;
padding-left:84px;
```

Shorthand:

```css
padding:20px 23px 52px 84px;
```

Order:

```text
Top Right Bottom Left
```

Remember:

```text
TRBL
Top Right Bottom Left
```

---

### Width Properties

```css
width:fit-content;
max-width:100px;
```

Meaning:

```text
fit-content → width depends on content

max-width → maximum allowed width
```

---

## 📅 12 June 2026

# CSS Selectors & Pseudo Classes

### Universal Selector

```css
*{
  margin:0;
}
```

Selects every element.

---

### Descendant Selector

```css
div p{
  background:brown;
}
```

Meaning:

```text
Select all p elements inside div
```

---

### Attribute Selector

```css
a[target]{
  background:blueviolet;
}
```

Meaning:

```text
Select elements containing target attribute
```

---

### Adjacent Sibling Selector

```css
.parabox + p{
  background:goldenrod;
}
```

Meaning:

```text
Select immediate next sibling only
```

---

### Hover

```css
:hover
```

Triggered when mouse is over an element.

---

### Active

```css
:active
```

Triggered while mouse button is pressed.

---

### First Child

```css
p:first-child
```

Meaning:

```text
Paragraph must be first child
of its parent
```

---

### Selection Pseudo Element

```css
::selection
```

Changes selected text appearance.

---

### Selector Types Learned

```text
Universal Selector
Element Selector
Class Selector
Descendant Selector
Attribute Selector
Adjacent Sibling Selector
```

### Pseudo Classes Learned

```text
:hover
:active
:first-child
```

### Pseudo Elements Learned

```text
::selection
```

---

## 📅 13 June 2026

# Text & Font Properties

### Text Alignment

```css
text-align:center;
text-align:justify;
```

---

### Text Align Last

```css
text-align-last:center;
```

Controls alignment of last line.

---

### Text Decoration

```css
text-decoration-line
text-decoration-color
text-decoration-style
text-decoration-thickness
```

Example:

```css
text-decoration-line:line-through;
text-decoration-style:wavy;
```

---

### Text Indent

```css
text-indent:30px;
```

Moves first line inward.

---

### Letter Spacing

```css
letter-spacing:4px;
```

Space between letters.

---

### Word Spacing

```css
word-spacing:20px;
```

Space between words.

---

### Line Height

```css
line-height:50px;
```

Space between lines.

---

### Text Transform

```css
text-transform:uppercase;
text-transform:lowercase;
text-transform:capitalize;
```

---

### Text Shadow

Syntax:

```css
text-shadow:
horizontal
vertical
blur
color;
```

Example:

```css
text-shadow:2px 2px 3px gray;
```

---

### Direction

```css
direction:ltr;
direction:rtl;
```

Controls text direction.

---

### Font Family

```css
font-family:
Arial,
Helvetica,
sans-serif;
```

Fallback system:

```text
First unavailable?
Use second.
Still unavailable?
Use third.
```

---

### Font Size

```css
font-size:50px;
```

Controls text size.

---

### Font Weight

```css
font-weight:100;
font-weight:400;
font-weight:700;
font-weight:900;
```

Common Values:

```text
400 = normal
700 = bold
900 = extra bold
```

---

### Font Style

```css
font-style:normal;
font-style:italic;
font-style:oblique;
```

---

### Font Variant

```css
font-variant:small-caps;
```

Converts lowercase letters into small capital letters.

---

## 🔥 Quick Revision Sheet

### CSS Priority

```text
!important
↓
Inline
↓
Internal
↓
External
```

### Box Model

```text
Content + Padding + Border
```

### Border Box

```text
Width includes:
Content + Padding + Border
```

### Padding Order

```text
Top Right Bottom Left
```

### Selector Types

```text
Universal
Element
Class
Descendant
Attribute
Adjacent Sibling
```

### Pseudo Classes

```text
:hover
:active
:first-child
```

### Pseudo Elements

```text
::selection
```

### Font Properties

```text
font-family
font-size
font-weight
font-style
font-variant
```

### Text Properties

```text
text-align
text-align-last
text-indent
letter-spacing
word-spacing
line-height
text-transform
text-shadow
text-decoration
direction
```
