# CSS Rule

SCSS / CSS 使用

### クラス名のルール

```scss

.classname {
	&__title {
		font-size: 24px;
		font-wight: bold;
	}
	&__ul {
		font-size: 0;
		letter-spacing: 0;
	}
	&__li {
		display: inline-block;
		width: 50%;
	}
}


```
# マークアップルール beta版


### 仮メモ

```html
<ul class="side-nav__list--small">
```
そのものを装飾するときは--small

```html
<ul class="side-nav__list__small">
```
その子供を装飾するときは__small



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
<<<<<<< Updated upstream
    <ul class="side-nav__list">
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
    </ul>
=======
	<ul class="side-nav__list">
		<li>
			<a>
				<figure></figure>
				<p></p>
			</a>
		</li>
	</ul>
>>>>>>> Stashed changes
</header>
```
```sass
.side-nav {
    &__list {
    
        li {
	    ...
	}
	
        a {
	    ...
	}
	
	figure {
	    ...
	}
	
	p {
	    ...
	}
    }
}
```

### sass設計理論

<<<<<<< Updated upstream
#### フォルダ構造

```
base.scss
  _color.scss

utill.scss  # 便利ツール
  _mixin.scss

component.scss

  header
  footer
  container
  .hero
  ...
  
```

=======


style.scss
header
footer
container
.hero

@import
base.scss
_color.scss
utill.scss
_mixin.scss
便利ツール
>>>>>>> Stashed changes


### ...
