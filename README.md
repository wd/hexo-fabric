hexo-fabric
===========

hexo-fabric is a theme for [hexo](https://github.com/tommy351/hexo), fork from [fabric](http://github.com/panks/fabric) by [Pankaj Kumar](http://panks.me) for octopress.

You can visit [my blog](http://wdicc.com) to preview.

### how to install

Like all other theme, execute the following command, and set `theme` in `_config.yml` to `hexo-fabric`。
```
$ git clone https://github.com/wd/hexo-fabric themes/hexo-fabric
$ hexo generate
```

There some settings in `theme/hexo-fabric/_config.yml` you may want to set.

### highlight theme
Only test on hexo 2.4.4, and highlight.js 0.8, maybe not work in other version.

Visit https://github.com/isagalaev/highlight.js/tree/master/src/styles to download a thtme into `source/stylesheets/hljs.css`. You can visit http://highlightjs.org/static/test.html  to select your fav theme.

Use vim open hljs.css you download, and then:
```
:%s/.hljs-/.code ./g
:wq
```

Then regenerate your site.

### TODO
- do not support pagination for archive, tags
- do not support category
- titlecase, line_number, date_format settings support
- robots, sitemap not work

Recommand you set like following in your `_config.yml`.
```
# Archives
## 2: Enable pagination
## 1: Disable pagination
## 0: Fully Disable
archive: 1
category: 0
tag: 1
```

Since hexo 3.x changed it's architechure and config file, to disable pagination for archive, you should put following settings in your `_config.yml`.
```
archive_generator:
  per_page: 1000  # a big number
  yearly: true
  monthly: true
```
