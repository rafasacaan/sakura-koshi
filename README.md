# sakura koshi (桜格子)

A minimalist grid system extension for [Sakura.css](https://github.com/oxalorg/sakura), following its philosophy of simplicity and elegance. The name "Koshi" (格子) means lattice or grid in Japanese, complementing Sakura's (桜, cherry blossom) theme.

## Features

- Lightweight grid system (~2KB minified)
- Maintains Sakura's minimalist philosophy
- Responsive and mobile-first
- Uses modern Flexbox
- No conflicts with Sakura's existing styles
- Simple class-based system

## Installation

1. First, include Sakura.css in your project
2. Then add Sakura Koshi after it:

```html
<link rel="stylesheet" href="https://unpkg.com/sakura.css/css/sakura.css">
<link rel="stylesheet" href="sakura-koshi.css">
```

## Usage

### Basic Grid

Create a basic grid using the `.container`, `.grid`, and `.col-*` classes:

```html
<div class="container">
  <div class="grid">
    <div class="col-6">Half width</div>
    <div class="col-6">Half width</div>
  </div>
</div>
```

### Column Sizes

Choose from 12 column sizes:
- `.col-1` (8.33%)
- `.col-2` (16.66%)
- `.col-3` (25%)
- `.col-4` (33.33%)
- `.col-6` (50%)
- `.col-12` (100%)
... and more

### Grid Gaps

Control spacing between grid items:
```html
<div class="grid grid-gap-2">
  <div class="col-4">Column</div>
  <div class="col-4">Column</div>
  <div class="col-4">Column</div>
</div>
```

Available gap sizes:
- `.grid-gap-0` (no gap)
- `.grid-gap-1` (0.5rem)
- `.grid-gap-2` (1rem)
- `.grid-gap-3` (1.5rem)

### Alignment

Horizontal alignment:
```html
<div class="grid grid-center">
  <!-- Centers content horizontally -->
</div>
```

Available alignment classes:
- `.grid-center`
- `.grid-start`
- `.grid-end`
- `.grid-between`
- `.grid-around`

Vertical alignment:
- `.grid-items-center`
- `.grid-items-start`
- `.grid-items-end`

### Responsive Behavior

All grids automatically stack on mobile devices (below 684px width to match Sakura's breakpoints).

## Example Layouts

### Three Column Layout
```html
<div class="container">
  <div class="grid grid-gap-2">
    <div class="col-4">
      <h3>Column 1</h3>
      <p>Content here</p>
    </div>
    <div class="col-4">
      <h3>Column 2</h3>
      <p>Content here</p>
    </div>
    <div class="col-4">
      <h3>Column 3</h3>
      <p>Content here</p>
    </div>
  </div>
</div>
```

### Sidebar Layout
```html
<div class="container">
  <div class="grid grid-gap-2">
    <div class="col-3">
      <!-- Sidebar -->
      <nav>
        <ul>
          <li><a href="#">Link 1</a></li>
          <li><a href="#">Link 2</a></li>
        </ul>
      </nav>
    </div>
    <div class="col-9">
      <!-- Main content -->
      <h2>Main Content</h2>
      <p>Your content here...</p>
    </div>
  </div>
</div>
```

## Contributing

Feel free to open issues or submit pull requests on GitHub.

## License

MIT License (same as Sakura.css)

## Credits

Inspired by and designed to complement [Sakura.css](https://github.com/oxalorg/sakura) by [oxalorg](https://github.com/oxalorg).
