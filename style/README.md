# CSS Rule

SCSS / CSS 使用

### クラス名のルール

```scss

.classname {
	font-size: 50px;
}

.page-title__red {
	font-size: 50px;
	color: red;
}

```
# マークアップルール beta版

### タブ幅は4スペ

### ファーストビューのclass名は"hero"

```html
<div class="hero">
	<ul class="hero__slider">
		<li class="hero__list"></li>
		<li class="hero__list"></li>
		<li class="hero__list"></li>
	</ul>
</div>
```

### sassの階層は三つまで

```html
<header class="side-nav">
	<ul class="side-nav__list">
		<li></li>
		<li></li>
		<li></li>
		<li></li>
		<li></li>
		<li></li>
	</ul>
</header>
```
```sass
.side-nav {
	&__list {
		li {
		}
		a {
		}
		figure {
		}
		p {
		}
	}
}

```
### sass設計理論

base.scss
_color.scss

utill.scss
_mixin.scss
便利ツール

component.scss
header
footer
container
.hero




### ...