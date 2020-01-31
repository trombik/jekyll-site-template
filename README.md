## Features

* i18n support by [`jekyll-polyglot`](https://github.com/untra/polyglot)
* `Sitemap` support by [`jekyll-sitemap`](https://github.com/jekyll/jekyll-sitemap)
* [Twitter Card](https://developer.twitter.com/en/docs/tweets/optimize-with-cards/overview/abouts-cards) support ([validator](https://cards-dev.twitter.com/validator)

## Requirements

* `ImageMagick` 6.x (for `jekyll-responsive-image`)

## Usage

```
bundle install --path=~/.vendor/bundle
bundle exec jekyll browsersync
```
## `i18n`

[`polyglot`](https://github.com/untra/polyglot) is used to support i18n.

## `l10n` How-to

Create a new page, `News`, which is a page for `lang` `en`, and the default
for other language if no translated page is found. The page must have `lang`
and `permalink` in the front matter. The file name is `news.html`.

```yaml
---
layout: default
title: News
lang: en
permalink: news/
---
The content
```

Create a localized one for `lang` `ja`, `news.ja.html`.

```yaml
---
layout: default
title: News
lang: ja
permalink: news/
---
The localized content
```

If the page should be included in the navigation bar, add an item to `_data/navi_items.yml`.

```yaml
---
- name: Home
  href: /
- name: About
  href: /about/
- name: Products
  href: /products/
- name: Store
  href: /store/
- name: News
  href: /news/
```

## URLs

* [the staging site on S3](http://jekyll-aws.s3-website-ap-northeast-1.amazonaws.com/)

## Plug-ins to consider

## Links

### `jekyll`

* [Setting up a Living Styleguide in Jekyll](https://www.sitepoint.com/setting-up-a-living-styleguide-in-jekyll/)
* [Custom Tags in Liquid](https://thoughtbot.com/blog/custom-tags-in-liquid)
* [18F/18f.gsa.gov](https://github.com/18F/18f.gsa.gov) (a production
  repository using jekyll)

### `S3`

* [How do I use CloudFront to serve a static website hosted on Amazon S3?](https://aws.amazon.com/premiumsupport/knowledge-center/cloudfront-serve-static-website/)
* [Serving custom headers from static sites on CloudFront/S3 with Lambda@Edge](https://medium.com/@tom.cook/edge-lambda-cloudfront-custom-headers-3d134a2c18a2)
