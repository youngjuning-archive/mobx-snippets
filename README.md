# mobx-snippets

## mobx

```js
import { observable, action } from "mobx"
```

## mobx-file

```js
import { observable, action } from "mobx"

class ${1:ClassName} {
  @observable title = ''
}

export default ${1:ClassName}
```

## mobx-class

```js
class ${1:ClassName} {
  @observable title = ''
}
```

## mobx-observable

```js
@observable $1 = $2
```

## mobx-action

```js
@action ${1:boundClassMethod} = () => {
  $2
}
```

## mobx-runInAction

```js
runInAction(() => {
  $1
})
```

## mobx-react

```js
import { observer } from "mobx-react"
```

## mobx-react-native

```js
import { observer } from "mobx-react/native"
```

## mobx-rn-screen

```js
/* eslint no-useless-constructor:0 */
import React, { Component } from 'react'
import {
  View,
  Text,
  StyleSheet,
} from 'react-native'
import { observer } from 'mobx-react/native'

@observer
class ${1:MyComponent} extends Component {
  constructor(props) {
    super(props)
  }

  componentDidMount() {}

  render() {
    return (
      <View style={styles.container}>
        <Text>I am the ${1:MyComponent} component</Text>
      </View>
    )
  }
}

const styles = StyleSheet.create({
  container: {
    flex: 1,
  },
})
export default ${1:MyComponent}
```

## mobx-rn-component

```js
import React, { Component } from 'react'
import {
  View,
  Text,
  StyleSheet,
} from 'react-native'
import { observer } from 'mobx-react/native'

@observer
class ${1:MyComponent} extends Component {

  render() {
    return (
      <View style={styles.container}>
        <Text>I am the ${1:MyComponent} component</Text>
      </View>
    )
  }
}

const styles = StyleSheet.create({
  container: {
    flex: 1,
  },
})
export default ${1:MyComponent}
```

## mobx-rn-stateless

```js
import { observer } from 'mobx-react'
import React from 'react'
import { View, Text, StyleSheet } from 'react-native'
import PropTypes from 'prop-types'

function ${1:componentName}({ style }) {
  return (
    <View style={[styles.container, style]} />
  )
}

${1:componentName}.propTypes = {

}

${1:componentName}.defaultProps = {

}

const styles = StyleSheet.create({
  container: {},
})
export default observer(${1:componentName})
```

## mobx-rn-func

```js
const ${1:FuncName} = observer(({ ${2:props} }) => (
  <view />
))
```
