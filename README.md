# Instant Markup App
> A GUI way to make and transform your articles to Facebook Instant Articles

## Server side

Instant Markup App works with a JSON-LD script.

### JSON-LD Example for Articles

[Enabling Rich Snippets for Articles](https://developers.google.com/structured-data/rich-snippets/articles#examples)

```html
<script type="application/ld+json">
{
  "@context": "http://schema.org",
  "@type": "NewsArticle",
  "mainEntityOfPage":{
    "@type":"WebPage",
    "@id":"https://google.com/article"
  },
  "headline": "Article headline",
  "image": {
    "@type": "ImageObject",
    "url": "https://google.com/thumbnail1.jpg",
    "height": 800,
    "width": 800
  },
  "datePublished": "2015-02-05T08:00:00+08:00",
  "dateModified": "2015-02-05T09:20:00+08:00",
  "author": {
    "@type": "Person",
    "name": "John Doe"
  },
   "publisher": {
    "@type": "Organization",
    "name": "Google",
    "logo": {
      "@type": "ImageObject",
      "url": "https://google.com/logo.jpg",
      "width": 600,
      "height": 60
    }
  },
  "description": "A most wonderful article"
}
</script>
```
