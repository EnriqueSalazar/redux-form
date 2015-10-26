<ol class="breadcrumb">
  <li><a href="#/">Redux Form</a></li>
  <li><a href="#/api">API</a></li>
  <li class="active">Action Creators</li>
</ol>

# Action Creators

`redux-form` exports all of its internal action creators, allowing you complete control to dispatch any action
you wish. However, **it is *highly* recommended that you use the actions passed as props to your component
for most of your needs.**

### `blur(form:String, field:String, value:String)`

> Saves the value to the field.

### `change(form:String, field:String, value:String)`

> Saves the value to the field.

### `focus(form:String, field:String)`

> Marks the given field as `active` and `visited`.

### `initialize(form:String, data:Object)`

> Sets the initial values in the form with which future data values will be compared to calculate
`dirty` and `pristine`. The `data` parameter should only contain `String` values.

### `initializeWithKey(form:String, formKey, data:Object)`

> Used when editing multiple records with the same form component. Useful when 
[editing multiple records](#/examples/multirecord).

### `reset(form:String)`

> Resets the values in the form back to the values past in with the most recent `initialize` action.

### `startAsyncValidation(form:String)`

> Flips the `asyncValidating` flag `true`.

### `startSubmit(form:String)`

> Flips the `submitting` flag `true`.

### `stopSubmit(form:String, errors:Object)`

> Flips the `submitting` flag `false` and populates `submitError` for each field.

### `stopAsyncValidation(form:String, errors:Object)`

> Flips the `asyncValidating` flag `false` and populates `asyncError` for each field.

### `touch(form:String, ...fields:String)`

> Marks all the fields passed in as `touched`.

### `untouch(form:String, ...fields:String)`

> Resets the 'touched' flag for all the fields passed in.

### `destroy(form:String)`

> Destroys the form, removing all its state.
