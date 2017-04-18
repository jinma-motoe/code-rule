# WS KANAZAWA コーディングルール


命名規則はBEMに遵守

```html

block
block--modifier
block__element
block__element--modifier

```

```html
//html

<div class="block">
	<div class="block__element"></div>
	<div class="block__element--modifier"></div>
</div>
<div class="block block--modifier">
	<div class="block__element"></div>
</div>

```

```scss
//sass

.block {
	&--modifier {
	}
	&__element {
		&--modifier {
		}
	}
}

```
