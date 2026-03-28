# Booking Widget

The Hosted Collection uses Hostaway's JavaScript booking widget embedded directly into Squarespace via a Code Block. The widget surfaces live availability and routes guests into the Hostaway reservation flow.

## Configuration

```javascript
<script>
  window.hostaway = {
    baseUrl: 'https://book.thehostedcollection.com/',
    color: '#C8644A',
    font: 'DM Sans',
  };
</script>
<script src="https://d2q3n06xhbi0am.cloudfront.net/widget.js"></script>
```

## Squarespace placement

- Add a **Code Block** to the page where the widget should appear
- Paste the full script into the block
- The widget script must load at the **bottom** of the last Code Block on the page — loading it mid-page causes rendering issues in Squarespace's block-based layout
- The widget is responsive and adapts to the Squarespace column width

## Notes

- `baseUrl` must match the Hostaway direct booking domain exactly, including the trailing slash
- `color` sets the primary CTA button color — use the brand espresso/terracotta `#C8644A`
- `font` must match a Google Font name exactly as it appears in the Google Fonts library
