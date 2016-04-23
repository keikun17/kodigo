#REDUX

## Reducers

A pure function

used to create a store (using the createStore function from Redux)

import { createStore } from 'redux'

const someReducer = (state, action) {
  switch(action.type) {
    case "SOME ACTION":
      return state.some_state_attribute = "some mutation"
    default:
      state
  }
}

someStore = createStore(somereducer)

## combineReducers

```javascript
import { combineReducers } from 'redux'

const myApp = combineReducers({ reducerOne: reducerOne, reducerTwo: reducerTwo })
// or
const myApp = combineReducers({reducerOne, reducerTwo})

// Both are equivalent to :
// const myAppReducer = (state = {}, action ) => {
//  return {
//    reducerOne: reducerOne(state.reducerOne, action),
//    reducerTwo: reducerTwo(state.reducerTwo, action)
//  }
}
```
