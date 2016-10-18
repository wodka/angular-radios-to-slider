angular-radios-to-slider
===========
[![Bower version](https://badge.fury.io/bo/angular-radios-to-slider.svg)](http://badge.fury.io/bo/angular-radios-to-slider)

angular module for https://github.com/rubentd/radios-to-slider

### Installation

```
bower install angular-radios-to-slider --save
```

### Usage

add "radio.slider" to your modules and start using the directive.

### Example

```html
<html ng-app="app">
<body ng-controller="Controller as vm">
<radio-slider values="vm.values" ng-model="vm.options"></radio-slider>
</body>
</html>

<script>
angular.module('app', ['radio.slider']).controller('Controller', Controller);

function Controller() {
	var vm = this;

	vm.options = 'option4';

	vm.values = {
		'option1': '1 years',
		'option2': '2 years',
		'option3': '3 years',
		'option4': '4 years',
		'option5': '5+ years'
	};
}
</script>
```

