hexo-fabric
===========

hexo-fabric is a theme for [hexo](https://github.com/tommy351/hexo), fork from [fabric](http://github.com/panks/fabric) by [Pankaj Kumar](http://panks.me) for octopress.

You can visit [my blog](https://wdicc.com) to preview.

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

### tags cloud page

If you want to support tags cloud page, you should create a empty page use command `hexo  new page 'tags'`. And then change the title for this page to 'All Tags' or what you want, it will display at tags cloud page.

If you don't want this page, you can delete it from `themes/hexo-fabric/layout/_partial/custom/navigation.ejs`.

### TODO
- do not support category
- titlecase, line_number, date_format settings support
- robots, sitemap may not work

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
