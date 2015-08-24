[Kit Pearson Photography](pearsonhedshots.com)
=======================

This is my headshot photography site.

Built on [Jekyll] and based on the [Grayscale bootstrap theme](grayscale).

Hosted on Github pages, for which I am eternally grateful.

[jekyll]: http://jekyllrb.com/
[grayscale]: (http://ironsummitmedia.github.io/startbootstrap-grayscale/)

---------------

Development Notes

Depending on the environment couple changes need to be made to the css include statements.

1. The `baseurl` variable in `_config.yml` needs to be set for the given environment.
Production:
```
baseurl: "/photo_site"
```
Local dev:
```
baseurl: ""
```

2. The css reference to the background image needs:
On line 141 in `/_includes/css/grayscale.css` the `background: url` need to be set.
Production:
```
background: url(/photo_site/img/intro-bg.jpg)
```
Local dev:
```
background: url(/img/intro-bg.jpg)
```