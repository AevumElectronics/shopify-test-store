# shopify-test-store

Link: https://impossible-store-test-1.myshopify.com/
PW: chupeu

The newly created Web Component is:
sections/product-info-accordion.liquid

The video has been added through a custom liquid section 
that shows the video only if the product type is "shirt".

```
{% if product.type contains "shirt" %}
<style>.embed-container { position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden; max-width: 100%; } .embed-container iframe, .embed-container object, .embed-container embed { position: absolute; top: 0; left: 0; width: 100%; height: 100%; }</style><div class='embed-container'><iframe src='https://www.youtube.com/embed/AGcTCvn-a6g?autoplay=1' frameborder='0' allowfullscreen></iframe></div>
{% endif %}
```

The autoplay function is turned on but the video is hosted on youtube so on mobile it may not start (youtube/vimeo rules on mobile data).
For a fully working autoplay function load the video as a file.