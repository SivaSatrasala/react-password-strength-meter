# [React Password Strength Meter](https://github.com/SivaSatrasala/react-password-strength-meter)
React Component to display password strength meter with message and warning

## Dependencies
This Component is built using [Dropbox zxcvbn password strength estimator library](https://github.com/dropbox/zxcvbn)

## Installation & Usage

```
npm install react-password-strength-meter --save
```

## Password Strength Meter and values
This component will 'strength' meter as prop value (type: object).

```
strength default value :
strength : {
  0: "Worst ☹",
  1: "Bad ☹",
  2: "Weak ☹",
  3: "Good ☺",
  4: "Strong ☻"
}
```

### Include the Component

```
var React = require('react');
var PasswordStrengthMeter = require('react-password-strength-meter');

class Component extends React.Component {
  constructor(props){
    super(props);
    this.onChange = this.onChange.bind(this);
  }

  onChange(event){

  }

  render() {
    return <PasswordStrengthMeter passwordText={"Enter Password"} onChange={this.onChange} />;
  }
}
```

## License

MIT © [Siva Satrasala](https://github.com/SivaSatrasala)

