# React hooks

To manage variables in a React app, we could use one type of **React hook** \(a React function called `useState`\) which allows us to:

* _store_ the data within a variable
* _update_ the data using a function upon request

To use a hook more easily, we de-structure it when importing from `react`:

{% code title="app.js" %}
```jsx
import React, { useState } from 'react'
```
{% endcode %}

Then, we could use an `export default function` to use `useState`:

{% code title="app.js" %}
```jsx
import React, { useState } from 'react'

export default function myStateMachine() {

    const [ myState, setMyState ] = useState()

}
```
{% endcode %}

There, we do something called **array de-structuring** where we can re-use the **store variable** `myState` inside the rest of the function, as well as the **update function** `setMyState` ****to change the value of myState...

{% hint style="info" %}
Note that `myState` and `setMyState` 

* can have different names
  * \(e.g. `students` and `setStudents`\)
* however, a convention uses 
  * a `noun` for the store variable 
  * `set` plus `noun` for the update function
{% endhint %}



