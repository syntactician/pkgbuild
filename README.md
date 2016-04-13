# PKGBUILDs for Arch

#### How to use:

* Clone `~.build`
* Run:

```{sh}
for PKG in */; do
	(
		cd $PKG
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
* [Scrapy](http://scrapy.org/) for Python 3
    * [parsel](https://github.com/scrapy/parsel), a new Scrapy library
	* [pydispatch](https://pydispatcher.sourceforge.net) without Python 2
	  dependencies
