#  HTML & CSS Learning Journey


## 📅 Daily Log

| Day | Date | Topic | Status |
|-----|------|-------|--------|
| 01 | 10 June 2026 | CSS Priority — Inline vs Internal vs External | ✅ |
| 02 | 11 June 2026 | CSS Box Model — padding, margin, border-box | ✅ |

---

## 📖 Notes

### 📅 10 June 2026

#### CSS Priority
Priority Order:
```
!important  →  Highest
Inline CSS  →  Second
Internal CSS →  Third
External CSS →  Lowest
```

Example:
```html
<p style="color:red;">Hello</p>
```
```css
p { color: blue; }
```
> Output: **Red** — kyunki inline CSS wins

#### !important Override
```html
<p style="color:red;">Hello</p>
```
```css
p { color: blue !important; }
```
> Output: **Blue** — `!important` sabse upar hota hai, inline ko bhi override karta hai

---

### 📅 11 June 2026

#### CSS Box Model

Default behavior:
```css
box-sizing: content-box; /* browser ka default */
```
```
Actual Width = Content + Padding + Border

width:200px + padding:20px(×2) + border:10px(×2) = 260px
```

#### Border Box (recommended always use this)
```css
box-sizing: border-box; /* padding/border andar count hote hain */
```
```
width:200px + padding:20px + border:10px = still 200px ✅
```

#### Margin — element ke bahar space
```css
margin: auto;           /* center karta hai horizontally */
margin-top: 80px;
margin-bottom: 100px;
```

#### Padding — element ke andar space
```css
padding-top: 20px;
padding-right: 23px;
padding-bottom: 52px;
padding-left: 84px;

/* shorthand: top right bottom left */
padding: 20px 23px 52px 84px;
```

#### Width Properties
```css
width: fit-content;   /* content jitna bada, utna hi wide */
max-width: 100px;     /* is se zyada wide kabhi nahi hoga */
```

---
