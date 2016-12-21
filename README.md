# react-native-indicator

[![npm](https://img.shields.io/npm/dt/express.svg)](https://www.npmjs.com/package/react-native-indicator) ![react-native](https://img.shields.io/badge/react--native-0.38-brightgreen.svg) [![VersionEye](https://img.shields.io/versioneye/d/ruby/rails.svg)](https://github.com/wangdicoder/react-native-indicator) [![npm](https://img.shields.io/npm/l/express.svg)](https://www.npmjs.com/package/react-native-indicator)

A useful indicator component for React Native

<img src="/screenshot/ss1.gif" width="372" height="666" />
<img src="/screenshot/ss2.gif" width="372" height="666" />
<img src="/screenshot/ss3.gif" width="372" height="666" />
<img src="/screenshot/ss4.gif" width="372" height="666" />

## Installation

Make sure that you are in your React Native project directory and run:
```
$ npm install react-native-indicator --save 
```

### Android

It works, have fun!

### iOS

Add ```ART.xcodeproj``` from ```node_modules/react-native/React/Libraries/ART``` to your Libraries then link ```libART.a```. To see more details about **Linking Libraries**, jump to [this](https://facebook.github.io/react-native/docs/linking-libraries-ios.html).

## Usage

Import react-native-indicator as a JavaScript module:
```
import {CirclesLoader, PulseLoader, TextLoader, DotsLoader, ...} from 'react-native-indicator';
```

Here is currently available types: 

- [PulseLoader](#pulseLoader)
- [DotsLoader](#dotsLoader)
- [TextLoader](#textLoader)
- [BubblesLoader](#bubblesLoader)
- [CirclesLoader](#circlesLoader)
- [BreathingLoader](#breathingLoader)
- [RippleLoader](#rippleLoader)
- [LinesLoader](#linesLoader)
- [MusicBarLoader](#musicBarLoader)
- [EatBeanLoader](#eatBeanLoader)
- [DoubleCircleLoader](#doubleCircleLoader)
- [RotationCircleLoader](#rotationCircleLoader)
- [RotationHoleLoader](#rotationHoleLoader)
- [CirclesRotationScaleLoader](#circlesRotationScaleLoader)
- [NineCubesLoader](#nineCubesLoader)
- [LineDotsLoader](#lineDotsLoader)

[TOC]

```
render(){
    return(
        <View>
            <CirclesLoader />
            <TextLoader text="Loading" />
        </View>
    ); 
}
```

## Props

##### PulseLoader

| prop | type | default | description |
| ---- | ---- | ---- | ---- |
| size | number | 30 | circle's size |
| color | string | '#1e90ff' | indicator's color |
| frequency | number | 1000 | scale's frequency |


##### DotsLoader

| prop | type | default | description |
| ---- | ---- | ---- | ---- |
| size | number | 10 | dot's size |
| color | string | '#1e90ff' | indicator's color |
| betweenSpace | number | 5 | distance between two dots |


##### TextLoader

| prop | type | default | description |
| ---- | ---- | ---- | ---- |
| text | string | 'Loading' | contents |
| textStyle | style | inherited | text's style |


##### BubblesLoader

| prop | type | default | description |
| ---- | ---- | ---- | ---- |
| size | number | 40 | circle's size |
| color | string | '#1e90ff' | indicator's color |
| dotRadius | number | 10 | each dot's size |


##### CirclesLoader

| prop | type | default | description |
| ---- | ---- | ---- | ---- |
| size | number | 40 | circle's size |
| color | string | '#1e90ff' | indicator's color |
| dotRadius | number | 8 | each dot's size |


##### BreathingLoader

| prop | type | default | description |
| ---- | ---- | ---- | ---- |
| size | number | 10 | circle's size |
| color | string | '#1e90ff' | indicator's color |
| strokeWidth | number | 3 | outline width |
| frequency | number | 800 | scale's frequency |


##### RippleLoader

| prop | type | default | description |
| ---- | ---- | ---- | ---- |
| size | number | 10 | circle's size |
| color | string | '#1e90ff' | indicator's color |
| strokeWidth | number | 3 | outline width |


##### LinesLoader

| prop | type | default | description |
| ---- | ---- | ---- | ---- |
| color | string | '#1e90ff' | indicator's color |
| barWidth | number | 5 | each bar's width |
| barHeight | number | 40 | each bar's height |
| barNumber | number | 5 | the number of bar |
| betweenSpace | number | 2 | distance between two bars |


##### MusicBarLoader

| prop | type | default | description |
| ---- | ---- | ---- | ---- |
| color | string | '#1e90ff' | indicator's color |
| barWidth | number | 3 | each bar's width |
| barHeight | number | 30 | each bar's height |
| betweenSpace | number | 5 | distance between two bars |


##### EatBeanLoader

| prop | type | default | description |
| ---- | ---- | ---- | ---- |
| color | string | '#1e90ff' | indicator's color |
| size | number | 30 | indicator's size |


##### DoubleCircleLoader

| prop | type | default | description |
| ---- | ---- | ---- | ---- |
| size | number | 30 | circle's size |
| color | string | '#1e90ff' | indicator's color |


##### RotationCircleLoader

| prop | type | default | description |
| ---- | ---- | ---- | ---- |
| size | number | 30 | indicator's size |
| color | string | '#1e90ff' | indicator's color |
| rotationSpeed | number | 800 | rotation speed |


##### RotationHoleLoader

| prop | type | default | description |
| ---- | ---- | ---- | ---- |
| size | number | 40 | indicator's size |
| color | string | '#1e90ff' | indicator's color |
| rotationSpeed | number | 800 | rotation speed |
| strokeWidth | number | 8 | circle outline's width |


##### CirclesRotationScaleLoader

| prop | type | default | description |
| ---- | ---- | ---- | ---- |
| size | number | 50 | indicator's size |
| color | string | '#1e90ff' | indicator's color |


##### NineCubesLoader

| prop | type | default | description |
| ---- | ---- | ---- | ---- |
| size | number | 20 | each cube's size |
| color | string | '#1e90ff' | indicator's color |


##### LineDotsLoader

**warning:** *this indicator will occupy a whole horizontal space automatically, which means you don't need to set any center props. Just keeping the direction of its parent View is vertical.*

| prop | type | default | description |
| ---- | ---- | ---- | ---- |
| size | number | 10 | dot's size |
| color | string | '#1e90ff' | indicator's color |
| dotsNumber | number | 5 | the number of dots |
| betweenSpace | number | 5 | distance between two dots |

## License

MIT