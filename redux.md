#REDUX

combineReducers

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

