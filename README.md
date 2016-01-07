![screenshot](https://cloud.githubusercontent.com/assets/3277634/12009566/4c2cd29a-acb8-11e5-9ddd-a66c6a105208.png)

## Install

``` bash
hexo init blog
cd blog
# grep -vE "hexo-renderer-ejs|hexo-renderer-stylus" package.json > tmpfile; mv tmpfile package.json
npm install
npm install --save hexo-renderer-jade hexo-renderer-sass hexo-autoprefixer hexo-generator-feed hexo-generator-sitemap hexo-browsersync
git clone https://github.com/haukurk/hexo-theme-slojplojs.git themes/slojplojs
```

## Enable Slojplojs Theme

Edit `_config.yml`, set `theme` field as `slojplojs`:

```yaml
theme: slojplojs
```

## Configuration

### Enable google analytics

Add the following to your `_config.yml` files:

```yaml
ga: Tracking Number
```

## Update

``` bash
cd themes/slojplojs
git pull
```

## Custom Blocks

### Partial posts on front page

Use ``<!-- more -->`` to define the cutting point of the article.

### Warning Block

![Warning block screenshot](https://cloud.githubusercontent.com/assets/9530963/11359678/489a510c-92b9-11e5-9256-341cef6999b6.png)

Usage: `<p class="tip">Lorem ipsum dolor sit</p>`

## License

MIT
