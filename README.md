## adapt

**A flutter plugin for adapting screen.Adapt IOS and Android.**

## APIS
> Adapt.init(int 750) Initialize the setup size
> Adapt.px(int 30)    Calculated dimensions
> Adapt.onepx()       get 1px
> Adapt.screenW()     get the devices width
> Adapt.screenH()     get the devices height
> Adapt.padTopH()     get the devices padding top
> Adapt.padBotH()     get the devices padding bottom

## Usage:

### Add dependency：
```js

dependencies:
  flutter:
    sdk: flutter
  
  adapt: ^0.0.1  // select the last version

```

### Add the following imports to your Dart code:

```js
import 'package:adapt/adapt.dart';

```

## Use：

### If your design is 750px.

```js

// Set text size.
new Text(
    'Hello World!',
    style: TextStyle(
         fontSize: Adapt.px(30),
     )
)

// Set container size.
new Container(width: Adapt.px(300),  
    height: Adapt.px(300),
)

// get 1px
new Container(
    decoration: new BoxDecoration(
          border: new Border(bottom:BorderSide(width: Adapt.one())),
    ),
)

```

### If your design is not 750px.

* Initialize the setup size.

```js

// For example, the design is 1000px. You can do it like this.

Adapt.init(1000);

// and then use px
new Text(
    'Hello World!',
    style: TextStyle(
        fontSize: Adapt.px(30),
    )
)

```













