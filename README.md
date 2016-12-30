chaidarun.com
=============

### license

all rights reserved, except where otherwise noted

### documentation

custom page variables

- description         = content for meta description
- headcss             = extra css for head
- headjs              = extra js for head
- h1                  = what should go inside h1 tags
- pagetitle           = what should go inside title tags
- secret              = true iff page should be published but not sitemapped

includes

- ga                  = google analytics js

layouts

- blank               = nothing but {{ content }}
- default             = page without timestamp/tags
- minimal             = complete head, empty body
- post                = page with timestamp/tags

sass partials

- normalize           = normalize.css reset
- twilight            = for pygments
- tipsy               = for tipsy plugin
- webfonts            = fonts

### workflow

developing

```bash
make watch
make serve
```

publishing

```bash
make build
make sync host=******
make sitemap token=******
```
