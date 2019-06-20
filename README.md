## react-stopwatch

<p align="center">
  <img src="https://github.com/Bajtas/bjts-react-stopwatch/blob/master/images/stopwatch.jpg?raw=true" alt="How component looks"/>
</p>

Very extensible, provides many hooks so you can use them to develop any custom behavior that you desire.
Shipped with basic CSS style!

This project was bootstrapped with [Create React App](https://github.com/facebookincubator/create-react-app).

## Usage

```javascript
import React, { Component } from 'react';
import './App.css';
import StopWatch from './StopWatch';

class App extends Component {
  render() {
    return (
      <div className="App">
        <StopWatch/>
      </div>
    );
  }
}

export default App;
```

### Props

```javascript
StopWatch.propTypes = {
  // custom classNames
  stopwatchClassName: PropTypes.string,
  timeContainerClassName: PropTypes.string,
  controlsClassName: PropTypes.string,
  playIconClassName: PropTypes.string,
  pauseIconClassName: PropTypes.string,
  resetIconClassName: PropTypes.string,
  renderControls: PropTypes.element, // custom render function for controls section
  hideHours: PropTypes.bool, // hide hours
  hideMinutes: PropTypes.bool, // hide minutes
  hideSeconds: PropTypes.bool, // hide seconds
  hideMilliseconds: PropTypes.bool, // hide milliseconds
  separators: PropTypes.arrayOf(PropTypes.string) // separators to use between hours/minutes/seconds/milliseconds
  // separator use example: [":"/*separatorBetweenHoursAndMinutes*/, ":"/*separatorBetweenMinutesAndSeconds*/, "."/*separatorBetweenSecondsAndMilliseconds*/]
};
```
