# @React Datepicker

A simple datepicker react/typescript component.

You can set an id, name, placeholder, a onChange callback,
className and a preselected value via props.

[See demo link](https://sankarbala.github.io/datepicker/)

## Installation

The package can be installed via npm or yarn:

```bash
npm install @sankarbala/datepicker
```

```bash
yarn add @sankarbala/datepicker
```

## Usage

```js
import { DatePicker } from "@sankarbala/datepicker";

const MyForm = ({ data }) => {
  const handleInputChanged = ({ e }) => {
    console.log(e.target.value);
  };
  <DatePicker
    id="birthday"
    name="birthday"
    onChange={handleInputChanged}
    value={"01/01/2000"}
    className="form-control"
  />;
};
```

## Props

**_id_** : an optional id for the datepicker \
**_name_** : an optional name for the datepicker input\
**_placeholder_** : a placeholder string (optional)\
**_value_** : set the value of the datepicker input (optional)\
**_onChange_** : a callback function that takes as argument {target}\
**_className_** : classes that takes as argument {target}
