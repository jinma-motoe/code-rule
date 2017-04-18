# WS KANAZAWA コーディングルール

## 命名規則はBEMに遵守

```html

block
block__element
block__element--modifier
block--modifier
block--modifier__element

```

```html

<div class="block">
	<div class="block__element"></div>
	<div class="block__element--modifier"></div>
</div>
<div class="block block--modifier">
	<div class="block__element"></div>
</div>

```

```scss

.block {
	&--modifier {
	}
	&__element {
		&--modifier {
		}
	}
}

```
