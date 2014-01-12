hexo-fabric
===========

fabric theme for hexo

### Set highlight theme

hexo >= 2.4.4, hack lib/util/highlight.js
```
hljs.configure({
  classPrefix: 'hljs-'
});
```

Then visit https://github.com/isagalaev/highlight.js/tree/master/src/styles to download a thtme into `source/stylesheets/hljs.css`

You can do like following to select your fav theme.
```
$ git clone https://github.com/isagalaev/highlight.js
$ cd highlight.js
$ python ./tools/build.py
$ open src/test.html
```

gem install sass
gem install compass

:%s/.hljs-/.code ./g
