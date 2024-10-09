## Development 

1. Run `npm install` or `npm i`

## Build library

1. Run `npm run build`

## Installation

TODO

## Usage

Import `@a11y/focus-trap` somewhere in your code and you're ready to go! Simply add the focus trap to your `html` and it'll be working without any more effort from your part.

```html
<focus-trap>
  <button>Button 1</button>
  <button>Button 2</button>
  <button>Button 3</button>
  <button>Button 4</button>
  <button>Button 5</button>
</focus-trap>
```

## API

The `focus-trap` element implements the following interface.

```typescript
interface IFocusTrap {
  // returns whether or not the focus trap is inactive.
  inactive: boolean;

  // returns whether the focus trap currently has focus.
  readonly focused: boolean;

  // focuses the first focusable element in the focus trap.
  focusFirstElement: (() => void);

  // focuses the last focusable element in the focus trap.
  focusLastElement: (() => void);

  // returns a list of the focusable children found within the element.
  getFocusableElements: (() => HTMLElement[]);
}
```

## License
	
Licensed under [MIT](https://opensource.org/licenses/MIT).
