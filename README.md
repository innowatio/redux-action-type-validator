[![npm version](https://badge.fury.io/js/redux-action-type-validator.svg)](https://badge.fury.io/js/redux-action-type-validator)
[![Build Status](https://travis-ci.org/innowatio/redux-action-type-validator.svg?branch=master)](https://travis-ci.org/innowatio/redux-action-type-validator)
[![codecov](https://codecov.io/gh/innowatio/redux-action-type-validator/coverage.svg?branch=master)](https://codecov.io/gh/innowatio/redux-action-type-validator)
[![Dependency Status](https://david-dm.org/innowatio/redux-action-type-validator.svg)](https://david-dm.org/innowatio/redux-action-type-validator)
[![devDependency Status](https://david-dm.org/innowatio/redux-action-type-validator/dev-status.svg)](https://david-dm.org/innowatio/redux-action-type-validator#info=devDependencies)

# redux-action-type-validator

Type validator for redux actions

##  Installation

```sh
npm i --save redux-action-type-validator
```

## Usage

```js
import {list, String} from "tcomb";

const typeofAction = actionTypeValidator(list(String));

export function action (payload) {
    typeofSelectSite(...arguments);
    return {
        type: "ACTION_TYPE",
        payload
    };
}

// Somewhere in your code
action(["some", "string", "here"]); // not throw

action("some"); // throw


```
