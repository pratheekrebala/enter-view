# enter-view.js

Dependency-free JavaScript library to detect when element enters into view. [See demo](https://russellgoldenberg.github.io/enter-view/).

## Usage

```
enterView({
	selector: '.class-name',
	trigger: function(el) {
		el.classList.add('entered');
	}
});
```

## Options

#### selector: [string] _required_

Takes a class or id element selector

#### trigger: [function] _required_

Callback function that returns the element that was triggered

#### offset: [string] _optional_ (defaults to 0)

A value from 0 to 1 of how far from the bottom of the viewport to offset the trigger by. 0 = top of element crosses bottom of viewport (enters screen from bottom), 1 = top of element crosses top of viewport (exits screen top).

#### once: [boolean] _optional_ (defaults to true)

Whether or not to trigger the callback once or every time.
