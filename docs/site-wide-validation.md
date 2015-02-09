# Site-Wide Validation

To validate HTML and/or CSS on a site, all you need to do is specify the starting URL. Here are the additional options that you can set.

![New site validation form](img/new-site-validation-form.png)

## Options

To validate a site, you can define:

* **Starting URL**. Our validation spider will visit this URL and its direct internal links, and validate those pages. Typically, you can enter the main URL of the site to validate, but it can be any URL from your site, or an XML sitemap.
* **Max. pages**. The maximum number of pages to validate. There's a hard limit of 2,000 pages per each site validation, but you'll typically want to set a much lower limit.
* **Deep link scraping**. By default, the validation spider will follow the internal links found, discovering more pages, until the max pages limit is reached or no more pages are found. This provides an easy way to submit a large site, but it's also slower than specifying exactly the URLs to validate with an XML sitemap.
* **HTML validation**. If enabled, each page will be validated for HTML conformance using the W3C validation software.
* **CSS validation**. If enabled, each page will be validated for CSS conformance using the W3C validation software.

## Performance tips

Validating a large site can take a considerable amount of time, so in order to get your results sooner, consider:

### Using an XML sitemap

You can provide an XML sitemap specifying the exact URLs to validate. If you do so, we won't need to crawl your site to discover the pages to validate, so we can start validating pages sooner.

You can [read about the XML sitemaps protocol here](http://www.sitemaps.org/protocol.html), but in short, all you need is to specify each URL in this format:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<urlset xmlns="http://www.sitemaps.org/schemas/sitemap/0.9">
  <url>
    <loc>http://example.com/page1</loc>
  </url>
  <url>
    <loc>http://example.com/page2</loc>
  </url>
  <url>
    <loc>http://example.com/page3</loc>
  </url>
</urlset>
```

You can generate this XML sitemap manually or by using a tool [like this one](https://www.xml-sitemaps.com/).

Using XML sitemaps leads to much faster site validations, but also lets you be more organized when validating large sites. For example, you can use different XML sitemaps for the different sections in a large site.

### Disabling deep link scraping

By default, our validation spider will follow the initial URLs found from the starting URL, and discover additional pages until it reaches the indicated maximum pages to validate.

If you don't need us to discover additional pages, you can disable this option. For example, when you're submitting an XML sitemap with an exact set of pages to validate.

### Validating a smaller set of pages

While it's tempting to try to validate sites in its entirety, in most cases that's unnecessary. For example, the [New York Times](https://www.google.com/?q=site:nytimes.com) site has over 33 million URLs, it would be impossible to validate the whole site. When you have a blog, or an online store, your site has easily thousands of pages, but most of them are using the same layout. Instead of validating each of them, consider building an XML sitemap with a sample of each different kind of page. You'll save credits and time.

### Validate HTML and CSS separately

If you're validating CSS, consider again that most of the pages will be using the same stylesheets, so it's unnecessary to validate hundreds of pages for CSS. Consider validating just a small set of pages.

Also, you can check HTML and CSS separately. For example, if you have a 300-page site, you could validate HTML on 300 pages (or less), and CSS on 5 pages (or probably, just 1 page!).
