# 📖 Complete CSS Selectors Cheatsheet

A comprehensive guide to all CSS selectors with definitions and examples. Perfect for beginners and pros looking for a quick reference.

---

## 📦 Basic Selectors

| Selector      | Description                                  | Example            |
|---------------|----------------------------------------------|--------------------|
| `*`           | Selects all elements                         | `* { margin: 0; }` |
| `element`     | Selects all `<element>` tags                  | `p { color: blue; }` |
| `.class`      | Selects all elements with the class           | `.btn { padding: 10px; }` |
| `#id`         | Selects a single element with the id          | `#header { background: red; }` |

---

## 🔗 Combinator Selectors

| Selector        | Description                                           | Example                      |
|-----------------|-------------------------------------------------------|------------------------------|
| `A B`           | Descendant: Selects all `B` inside `A`                | `div p { color: green; }`    |
| `A > B`         | Child: Selects direct children `B` of `A`             | `ul > li { list-style: none; }` |
| `A + B`         | Adjacent sibling: Selects `B` immediately after `A`   | `h1 + p { margin-top: 0; }`  |
| `A ~ B`         | General sibling: Selects all `B` after `A`            | `h1 ~ p { color: gray; }`    |

---

## 🎯 Attribute Selectors

| Selector         | Description                                                   | Example                             |
|------------------|---------------------------------------------------------------|-------------------------------------|
| `[attr]`         | Selects elements with the attribute                           | `[disabled] { opacity: 0.5; }`     |
| `[attr="value"]` | Selects elements with exact attribute value                   | `[type="text"] { border: 1px solid; }` |
| `[attr~="value"]`| Attribute contains word value                                  | `[title~="flower"] { color: pink; }` |
| `[attr|="value"]`| Attribute starts with value (exact or hyphenated)              | `[lang|="en"] { font-family: serif; }` |
| `[attr^="value"]`| Attribute starts with value                                    | `[href^="https"] { color: green; }` |
| `[attr$="value"]`| Attribute ends with value                                      | `[src$=".jpg"] { border-radius: 10px; }` |
| `[attr*="value"]`| Attribute contains value                                       | `[class*="btn"] { padding: 5px; }`  |

---

## 🎛 Pseudo-Classes

| Selector           | Description                                         | Example                              |
|--------------------|-----------------------------------------------------|--------------------------------------|
| `:hover`           | Styles when the user hovers                        | `a:hover { color: red; }`           |
| `:focus`           | Styles when element has focus                      | `input:focus { outline: none; }`    |
| `:first-child`     | Selects the first child                             | `p:first-child { font-weight: bold; }` |
| `:last-child`      | Selects the last child                              | `p:last-child { color: blue; }`     |
| `:nth-child(n)`    | Selects the nth child                               | `li:nth-child(2) { color: red; }`   |
| `:nth-of-type(n)`  | Selects the nth element of its type                 | `p:nth-of-type(2) { font-size: 20px; }` |
| `:only-child`      | Selects elements that are the only child            | `div:only-child { margin: 0 auto; }`|
| `:not(selector)`   | Selects everything except specified selector        | `div:not(.active) { opacity: 0.3; }`|

---

## 🎨 Pseudo-Elements

| Selector         | Description                                         | Example                                 |
|------------------|-----------------------------------------------------|-----------------------------------------|
| `::before`       | Inserts content before the element’s content        | `p::before { content: "★ "; }`          |
| `::after`        | Inserts content after the element’s content         | `p::after { content: " ✔"; }`           |
| `::first-line`   | Styles the first line of text                       | `p::first-line { font-weight: bold; }`  |
| `::first-letter` | Styles the first letter of text                     | `p::first-letter { font-size: 2em; }`   |
| `::selection`    | Styles selected text                                | `::selection { background: yellow; }`   |

---

## 📝 Quick Notes

✅ **Chaining selectors**: `div.highlighted.active:hover` targets only divs with both `.highlighted` and `.active` on hover.  
✅ **Universal selector** (`*`) is powerful but use cautiously for performance.  
✅ Attribute selectors are great for targeting dynamic or unknown elements.  

---

## 📚 Resources

- [CSS Selectors Reference (MDN)](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Selectors)
- [CSS-Tricks Selectors Guide](https://css-tricks.com/almanac/selectors/)
- [Specificity Calculator](https://specificity.keegan.st)

