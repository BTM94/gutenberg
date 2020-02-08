# AnglePicker

AnglePicker is a React component to render a UI that allows users to pick an angle.
Users can choose an angle in a visual UI with the mouse by dragging an angle indicator inside a circle or by directly inserting the desired angle in a text field.

## Usage


```jsx
import { useState } from '@wordpress/element';
import { AnglePicker } from '@wordpress/components';

const MyAnglePicker = () => {
	const [ angle, setAngle ] = useState();
	return <AnglePicker value={ angle } onChange={ setAngle } />;
};
```

## Props

The component accepts the following props.

### label

Label to use for the angle picker. If not set the a translated label "Angle" is used.

- Type: `String`
- Required: No

### value
The current value of the input.

- Type: `String | Number`
- Required: Yes

### onChange
A function that receives the new value of the input.

- Type: `function`
- Required: Yes
