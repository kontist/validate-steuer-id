# Description
> Package to validate German tax ID / steuer ID

# Installation
```
npm install validate-steuerid
```

```
yarn add validate-steuerid
```
# Usage
## As a module

You can either validate steuerId or generate a valid steuerId

```js
import { isSteuerIdValid, generateSteuerId, generateUniqueSteuerIds } from 'validate-steuerid'

isSteuerIdValid('65299970480')
// => false

isSteuerIdValid('65929970489')
// => true

isSteuerIdValid('26954371827')
// => true

generateSteuerId()
// => random steuerId string

generateUniqueSteuerIds(2)
// => array of 2 unique steuer id strings
```
## Shell
```shell
yarn generateUniqueSteuerIds 20
```

# Methods
## isSteuerIdValid(steuerId)
* ### Takes `steuerId`:
  - type: `string`
* ### Returns `boolean`

## generateSteuerId()
* ### Returns `string`

## generateUniqueSteuerIds(numberOfSteuerIds)
* ### Takes `numberOfSteuerIds`:
  - type: `number`
* ### Returns `Array`:
  - type: `string`

<br>

# References
For developing the algorithm, we referenced the European Commission's TIN check modules stated [here](https://ec.europa.eu/taxation_customs/tin/#/check-tin).

<br>

---

*THE USE OF THE GENERATOR METHOD IS INTENDED FOR TESTING PURPOSES ONLY. THE NUMBERS GENERATED BY IT ARE COMPLETELY RANDOM AND ARE NOT MEANT TO BE USED IN ANY OFFICIAL CAPACITY.*
