# Squarespace Custom Code

Custom code used across the Squarespace site for The Hosted Collection.

## Footer — inline style fix

Squarespace's footer renders inconsistently across templates when custom fonts are applied. Use inline styles on the footer wrapper to force consistent rendering:

```html
<div style="font-family: 'DM Sans', sans-serif; font-size: 14px; color: #3B2A1A; letter-spacing: 0.02em;">
  <!-- footer content -->
</div>
```

## Google Fonts import

Add to **Settings → Advanced → Code Injection → Header**:

```html
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:ital,wght@0,300;0,400;1,300&family=DM+Sans:wght@300;400;500&display=swap" rel="stylesheet">
```

## CSS overrides

Add to **Design → Custom CSS**:

```css
/* Headings */
h1, h2, h3 {
  font-family: 'Cormorant Garamond', serif;
  font-weight: 300;
  letter-spacing: 0.04em;
}

/* Body */
body, p, a {
  font-family: 'DM Sans', sans-serif;
  font-weight: 300;
}
```
