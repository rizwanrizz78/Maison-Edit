# Maison Édit Blogger Theme

A production-ready, magazine-style fashion blog theme designed for Blogger.com.

## Manual Setup Placeholders

Before finalizing the theme setup, you need to replace a few placeholder blocks in the HTML view (Theme > Edit HTML). Search for `[REPLACE:` to find them.

1. **Google Search Console**: Uncomment and replace the meta tag value with your verification string.
2. **Google Analytics (GA4)**: Uncomment and replace `G-XXXXXXXXXX` with your actual tracking ID.
3. **Author Bio Block**: Find the `<div class='author-bio-block'>` in the XML. Replace the placeholder avatar image URL (`https://via.placeholder.com/150`) and the placeholder description text.

## Widget IDs Explained

When you navigate to the **Layout** tab in Blogger, these are the custom-styled widgets you will interact with:

- **Header1**: Your blog title and optional description.
- **PageList1**: The navigation menu links. You can add, edit, or remove links here, and they will populate the header navigation (and slide-out menu on mobile).
- **Blog1**: The main feed of posts.
- **HTML1**: A generic HTML widget in the sidebar area.
- **LinkList1**: The footer navigation links. Used for pages like Privacy Policy, Contact, or Affiliate Disclosures. If empty, the theme injects placeholder links.

## Content Snippets for Post Editor

Because Blogger cannot render complex theme components inside the post body editor, this theme uses pre-styled HTML snippets. You can copy and paste these directly into your post editor while in **HTML View** (not Compose View). The CSS defined in the theme will automatically style them.

### 1. The Product Card

Use this block to embed products with affiliate links. It is fully responsive and supports an image, title, short description, and CTA button.

```html
<div class="me-product-card">
  <div class="me-product-image-wrap">
    <!-- Replace src with your product image URL -->
    <img src="https://via.placeholder.com/300" alt="Product Name" loading="lazy" />
  </div>
  <div class="me-product-info">
    <h3 class="me-product-title">Designer Handbag</h3>
    <p class="me-product-desc">A timeless, structured leather bag perfect for transitioning from day to night. Available in three neutral colors.</p>
    <!-- Replace href with your affiliate link -->
    <a href="https://your-affiliate-link.com" class="me-product-btn" target="_blank" rel="nofollow noopener">Shop Now - $450</a>
  </div>
</div>
```

### 2. Affiliate Disclosure

A subtle, nicely formatted box to place near the top of your post or right before a product grid to comply with FTC/affiliate guidelines.

```html
<div class="me-affiliate-disclosure">
  This post contains affiliate links. If you use these links to buy something we may earn a commission. <a href="/p/affiliate-disclosure.html">Read our full disclosure here</a>.
</div>
```
