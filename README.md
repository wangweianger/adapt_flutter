## adapt

**A flutter plugin for adapting screen.Adapt IOS and Android.**

## Usage:

### Add dependency：
```js

dependencies:
  flutter:
    sdk: flutter
  
  adapt: ^0.0.1  // select last version

```

### Add the following imports to your Dart code:

```js
import 'package:adapt/adapt.dart';

```

## Use：

### If your design is Figure 750 px.

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

