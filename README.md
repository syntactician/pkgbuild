# PKGBUILDs for Arch

#### How to use:

* Clone repository
* Run (in repository):

```{sh}
for PKG in */; do
	(
		cd $PKG
		makpkg -sri
	)
done
```

#### Contents:

* [dmenu](http://dmenu.suckless.org) with
  [Seoul256](https://github.com/junegunn/seoul256.vim) colors
* [slock](http://tools.suckless.org/slock) with Seoul256 colors
* [st](http://st.suckless.org) with Seoul256 colors, padding, and larger
  text
* [Scrapy](http://scrapy.org/) for Python 3
    * [parsel](https://github.com/scrapy/parsel), a new Scrapy library
	* [pydispatch](https://pydispatcher.sourceforge.net) without Python 2
	  dependencies
* [ChatterBot](https://pypi.python.org/pypi/ChatterBot), a Python dialog engine
	* [fuzzywuzzy](https://pypi.python.org/pypi/fuzzywuzzy), for fuzzy string matching
	* [jsondatabase](https://pypi.python.org/pypi/jsondatabase), a Python database format
	* [python-forecast.io](https://github.com/ZeevG/python-forecast.io), a Python wrapper for the [Forecast.io](http://forecast.io) API
	* [TextBlob](https://github.com/sloria/TextBlob), a library for textual processing
