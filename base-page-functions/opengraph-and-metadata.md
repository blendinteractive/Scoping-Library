# Opengraph, Metadata, and Schema.org

### Scope

We will cover the Apple Touch Icon, Favicon, Safari Pinned Tab (see rest of this page).

## Functional Specifications

### Gitlab Repository with Examples

[https://gitlab.blendinteractive.com/chad.thoreson/meta-html](https://gitlab.blendinteractive.com/chad.thoreson/meta-html)

Set on one place on the site, these act as fallbacks/defaults for most meta and open graph information.

The Site Defaults on an Episerver site are set in the Settings Page.

Fields that fallback to site defaults are:

* Meta Title
* Meta Description
* Open Graph: Title
* Open Graph: Description
* Open Graph: Image

### Integrating Schema.org

* Talk about javascript note
* We will use schema.org to match existing fields, but we will not create&#x20;

### Content Model

#### Icons

Set at the template level, these appear on every page.

Apple Touch Icon

`<pre><link rel="apple-touch-icon" sizes="180x180" href="/sharemeta-static/apple-touch-icon.png">`

Favicon

`<link rel="icon" type="image/png" sizes="32x32" href="/sharemeta-static/favicon-32x32.png">`

Safari Pinned Tab

`<link rel="mask-icon" href="/sharemeta-static/safari-pinned-tab.svg" color="#5bbad5"></pre>`

#### Open Graph: Type

This is set at the template level and there’s no need to add a field for this content. Setting the type to "website" works for all pages, but some clients may want to set type to "article" for News pages types, etc.

`<pre><meta property="og:type" content="website"></pre>`

#### Twitter:Card Summary Large Image

Set at the template level. This is the same on every page.

`<pre><meta name="twitter:card" content="summary_large_image"></pre>`

#### Meta Title

Use page title with “| Site name” at the end

`<pre><title>Test Social Page | Site Name</title></pre>`

Site default

`<pre><title>Test Social Page</title></pre>`

#### Meta Description

`<pre><meta name="description" content="Page description. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nullam sed imperdiet lectus. Nulla at tempus erat." /></pre>`

* Use Meta Description
* Use Page Summary
* Truncated amount of body text
* Site default

#### Open Graph: Site Name

`<pre>meta name="og:site_name" content="Test Site Name" /></pre>`

Site default. This is the same on each page.

#### Open Graph: Title

Uses the Meta Title content.

`<pre><meta property="og:title" content="Testing OG"></pre>`

#### Open Graph: Description

Uses the Meta Description content.

`<pre><meta property="og:description" content="OG Desc. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nullam sed imperdiet lectus. Nulla at tempus erat."></pre>`

#### Open Graph: Image

`<pre><meta property="og:image" content="https://chad.thoreson.blend.ly/sharemeta-static/images/puffin.jpg"></pre>`

* Open Graph Image set on page.
* Fall back to Article type image.
* Fall back to Header image.
* Site default.

#### Open Graph: URL

Use the URL from the current page.

`<pre>meta property="og:url" content="https://chad.thoreson.blend.ly/sharemeta-static/base.html"></pre>`

### Estimate Hours

TK

### Build Plan

TK

### Testing Scenario

1. Ensure all pages have all the above Meta and Open Graph items above set, including Icons
2. Ensure that pages with no Meta Data set to properties are inheriting Meta Data from the Start page
3. Ensure that changing the Meta Data Properties on a page update the Meta Data for the page
4. Ensure Open Graph: Type is used correctly on specific page types (when within scope)

#### Social Media Testing

Test sharing the page on Social Media:

* Facebook: [https://developers.facebook.com/tools/debug/sharing](https://developers.facebook.com/tools/debug/sharing)
* LinkedIn: [https://www.linkedin.com/post-inspector/](https://www.linkedin.com/post-inspector/)
* Slack: Share in Slack to see what comes back
* Twitter: [https://twitter.com/login?redirect\_after\_login=https%3A%2F%2Fcards-dev.twitter.com%2Fvalidator](https://twitter.com/login?redirect\_after\_login=https%3A%2F%2Fcards-dev.twitter.com%2Fvalidator)
