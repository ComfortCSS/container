# ComfortCSS Container

Modern container system with container queries, fluid widths, and full-width sections.

## Installation

```bash
npm install @comfortcss/container @comfortcss/tokens
```

## Usage

```css
@import '@comfortcss/reset';
@import '@comfortcss/tokens';
@import '@comfortcss/container';
```

## Examples

### Basic container

```html
<div class="container">
    <h1>Hello, World!</h1>
</div>
```

### Width variants

```html
<div class="container container-sm">...</div>
<div class="container container-lg">...</div>
<div class="container container-full">...</div>
```

### Padding modifiers

```html
<div class="container container--padding-lg">...</div>
<div class="container container--padding-none">...</div>
```

## API

### Container classes

| Class | Description|
|-------|------------|
| `.container` | Base container with fluid max-width |
| `.container-xs`, `.container-sm`, `.container-md`, `.container-lg`, `.container-xl`, `.container-2xl` | Width variants |
| `.container-full` | 100% width, no max-width |
| `.container-fluid` | Fluid width with min/max constraints |

### Modifiers

| Class | Description|
|-------|------------|
| `.container--padding-{none,xs,sm,md,lg,xl}` | Padding size |
| `.container--center`, `.container--center-h`, `.container--center-v` | Alignment |
| `.container--bleed` | Bleed effect |
| `.container--nested` | Resets max-width and padding |

### Container query classes

| Class | Description|
|-------|------------|
| `.cq-adaptive` | Typography adapts to container width |
| `.cq-spacing` | Padding adapts to container width |
| `.cq-side-by-side` | Flex side-by-side layout |
| `.cq-image` | Image float based on container width |
| `.cq-sm-adaptive`, `.cq-md-adaptive`, `.cq-lg-adaptive` | Named container variants |

## Customization

Override any token from `@comfortcss/tokens`:

```css
:root {
    --breakpoint-sm: 480px;
    --breakpoint-xl: 1200px;
    --space-4: 1.5rem;
}
```

## Dependencies

- [`@comfortcss/tokens`](https://github.com/ComfortCSS/tokens)

## License

[MIT](LICENSE)
