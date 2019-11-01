# On/Off Switch 

By using [step-by-step](https://github.com/Noahsok/React-JS-core-principles/tree/master/step-by-step) I built a stateful button that when clicked will be "turned" off or on.

#### Refactoring:
There is a cleaner and more responsive way to refactor this code. However, this is a good start to understand and see how a stateful component works and functions inside of a component.
#### example options:
You can see how the component works by looking at my 
- [CodePen](https://codepen.io/noahsok/pen/Exxbbbv?editors=0010)

## or:

See the code below:

```
class SwitchControl extends React.Component {
  constructor(props) {
    super(props);
    this.handleOnSwitch = this.handleOnSwitch.bind(this);
    this.handleOffSwitch = this.handleOffSwitch.bind(this);
      this.state = {isSwitchedOn: false};
  }
  handleOnSwitch() {
    this.setState({isSwitchedOn: true});
  }
  handleOffSwitch() {
    this.setState({isSwitchedOn: false});
  }
  
  render() {
    const isSwitchedOn = this.state.isSwitchedOn;
    let button;
    
    if (isSwitchedOn) {
      button = <OffSwitchButton onClick={this.handleOffSwitch} />;
    } else {
      button = <OnSwitchButton onClick={this.handleOnSwitch} />;
    }
    
    return (
      <div>
        <Switch isSwitchedOn={isSwitchedOn} />
        {button}
      </div>
    );
  }
}

function SwitchedOn(props) {
  return <h1>Switch is on!</h1>
}

function SwitchedOff(props) {
  return <h1>Switch is off!</h1>
}

function Switch(props) {
  const isSwitchedOn = props.isSwitchedOn;
  if (isSwitchedOn) {
    return <SwitchedOn />;
  }
  return <SwitchedOff />;
}

function OnSwitchButton(props) {
  return (
    <button onClick={props.onClick}>
    On!
    </button>
  );
}

function OffSwitchButton(props) {
  return (
    <button onClick={props.onClick}>
       off!
    </button>
  );
}

ReactDOM.render (
  <SwitchControl />,
  document.getElementById('root')
);
```


