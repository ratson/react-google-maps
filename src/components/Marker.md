## Usage

```js static
import { compose, withProps } from "recompose";

import {
  withGoogleMap,
  GoogleMap,
  Marker,
} from "react-google-maps";

import withScriptjs from "react-google-maps/lib/async/withScriptjs";

const CustomMap = _.flowRight(
  withProps({
    containerElement: <div style={{ height: `100%` }} />,
    mapElement: <div style={{ height: `100%` }} />,
  }),
  withScriptjs,
  withGoogleMap,
)(props => (
  <GoogleMap
    defaultZoom={8}
    defaultCenter={{ lat: -34.397, lng: 150.644 }}
  >
    <Marker
      position={{ lat: -34.397, lng: 150.644 }}
    />
  </GoogleMap>
));
```

### Map with a Marker

```
import { compose, withProps } from "recompose";

import {
  withGoogleMap,
  GoogleMap,
  Marker,
} from "react-google-maps";

import withScriptjs from "react-google-maps/lib/async/withScriptjs";

const CustomMap = _.flowRight(
  withProps({
    containerElement: <div style={{ height: `100%` }} />,
    mapElement: <div style={{ height: `100%` }} />,
  }),
  withScriptjs,
  withGoogleMap,
)(props => (
  <GoogleMap
    defaultZoom={8}
    defaultCenter={{ lat: -34.397, lng: 150.644 }}
  >
    <Marker
      position={{ lat: -34.397, lng: 150.644 }}
    />
  </GoogleMap>
));
```
