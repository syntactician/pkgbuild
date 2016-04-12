# PKGBUILDs for Arch

#### How to use:

* Clone as a subdirectory of `~.build`
* With GNU Stow:

```{sh}
for PKG in */; do
	stow $PKG
	(
		cd ../$PKG
		makepkg -sri
	)
done
```

* Without:

```{sh}
for PKG in */; do
	ln $PKG/$PKG ../$PKG
	(
		cd ../$PKG
		makpkg -sri
	)
done
```

#### Contents:

* [`dmenu`](http://dmenu.suckless.org) with
  [Seoul256](https://github.com/junegunn/seoul256.vim) colors
* [`slock`](http://tools.suckless.org/slock) with Seoul256 colors
* [`st`](http://st.suckless.org) with Seoul256 colors, padding, and larger
  text
* [Scrapy](http://scrapy.org/) [1.1.0rc1](https://pypi.python.org/pypi/Scrapy/1.1.0rc1) a [beta release](https://blog.scrapinghub.com/2016/02/04/python-3-support-with-scrapy-1-1rc1/) for Python 3
    * [parsel](https://github.com/scrapy/parsel), a new Scrapy library
