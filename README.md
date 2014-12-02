# www.epicodus.com

This is the source code for www.epicodus.com. It's built with the [Brace Tags](tags.brace.io) static site generator.

## Dependencies

Brace Tags is a Python package and requires Python 2 or 3.

To install Brace Tags:

```
$ easy_install brace-tags
$ easy_install watchdog
```

## Development

To run the site in development:

```
tags serve -w
```

Then visit `localhost:8000`.

## Deployment

The production www.epicodus.com site runs on [site44](site44.com). To build the site for production:

```
tags build -o ~/Dropbox/Apps/site44/www.epicodus.com/
```

Make sure to expire the cache in Cloudflare, as all content is cached.
