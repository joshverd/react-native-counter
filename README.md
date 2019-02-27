React Native Formatted Counter
====================

Forked from [react-native-counter](https://github.com/Kerumen/react-native-counter), adds support for a 'formatter' prop. You can use the formatter to modify the final displayed value of the counter.

Simple counter component for [React Native](http://facebook.github.io/react-native/)
inspired by [react-count-to](https://github.com/MicheleBertoli/react-count-to)
and [react-counter](https://github.com/saebekassebil/react-counter).

![gif](http://i.giphy.com/l4Jz4MOLaWYU61Oso.gif)

# Installation

```bash
npm install --save react-native-formatted-counter
```

# Usage

```javascript
import Counter from 'react-native-counter';

<Counter
  end={}                        // REQUIRED End of the counter
  start={0}                     // Beginning of the counter
  time={1000}                   // Duration (in ms) of the counter
  digits={0}                    // Number of digits after the comma
  easing="linear"               // Easing function name
  onComplete={}                 // Callback when the counter is completed
  style={}                      // Custom style
  formatter={(data) => {        // Custom Formatter - returned value is displayed
    return `$${data}`;
  }}
/>
```

The easing prop is a string corresponding to one of any function from [eases](https://github.com/mattdesl/eases).

# License

MIT
