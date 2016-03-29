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
