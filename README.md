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

## Deployment

To build the site for production:

```
tags build
```

Then copy the contents of `_site` to production.
