This folder is used for storing project styles.

In this project, we use BEM methodology for writing styles and organize the file structure according to BEM Nested.

Syntax:

- elements are separated from the blocks with a double underscore `__`
- modifiers are separated from blocks or elements by a single underscore `_`
- for the compound name of block or elements, we use a hyphen `-`

### Basic BEM Nested Structure
```bash
blocks/
  header/                             # Directory of the header block
    header.css                        # CSS for the header block
    __title/                          # Subdirectory of the header__title element
      header__title.css               # CSS for the header__title element
    __main-illustration/              # Subdirectory of the header__main-illustration element
      header__main-illustration.css   # CSS for the header__main-illustration element
```

### Key-Value modifiers
```bash
blocks/
  logo/                               # Directory of the logo block
    logo.css                          # CSS for the logo block
    _place/                           # Subdirectory of the logo modifier with key 'place'
      logo__place_header.css          # CSS for of the logo with the 'place' modifier set to 'header'
      logo__place_footer.css          # CSS for of the logo with the 'place' modifier set to 'footer'

```

### Boolean modifiers
```bash
blocks/
  link/                               # Directory of the link mix
    link.css                          # CSS for the link mix
    _active/                          # Subdirectory of the link mix with boolean modifier 'active'
      link_active.css                 # CSS for the active link mix
```

Please refer to the official [BEM](https://en.bem.info/methodology/quick-start/#introduction) or [BEM Nested](https://en.bem.info/methodology/quick-start/#file-structure) documentation for details if needed.

### Using media queries

For all components, we use the Desktop-first design approach, programming them initially for the desktop version, and subsequently adapting them to breakpoints: `1199px, 659px,` using `max-width` for media queries

Example:

```bash
.element {
   # styles for 1200px and above 
}

@media screen and (max-width: 1199px) {
  .element {
     # styles for screens from 660px to 1199px (excluding 1200px) 
  }
}

@media screen and (max-width: 659px) {
  .element {
    # styles for screens from 320px to 660px (excluding 600px)
  }
}
```
