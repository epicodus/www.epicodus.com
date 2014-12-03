# www.epicodus.com

This is the source code for www.epicodus.com. It's built with the [Brace Tags](tags.brace.io) static site generator.

## Dependencies

Brace Tags is a Python package and requires Python 2 or 3.

To install Brace Tags:

```
$ easy_install brace-tags
$ easy_install watchdog
```

## Use with Git

Brace Tags chokes on the `.git` folder, so after cloning, run:

```
mv .git _git  # Brace Tags ignores anything starting with _
echo "gitdir: _git" > .git
```

## Development

To run the site in development:

```
tags serve -w
```

Then visit `localhost:8000`. Brace Tags will automatically re-build the site for you as you make changes.

## Deployment

The production www.epicodus.com site runs on [site44](site44.com). To build the site for production:

```
tags build -o ~/Dropbox/Apps/site44/www.epicodus.com/
```

Make sure to expire the cache in Cloudflare, as all content is cached.
