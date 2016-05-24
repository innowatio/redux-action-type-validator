[![Build Status](https://travis-ci.org/innowatio/redux-action-type-validator.svg?branch=master)](https://travis-ci.org/innowatio/redux-action-type-validator)
[![Dependency Status](https://david-dm.org/innowatio/redux-action-type-validator.svg)](https://david-dm.org/innowatio/redux-action-type-validator)
[![devDependency Status](https://david-dm.org/innowatio/redux-action-type-validator/dev-status.svg)](https://david-dm.org/innowatio/redux-action-type-validator#info=devDependencies)

# redux-action-type-validator

Type validator for redux actions

## Usage

```js
import {list, String} from "tcomb";

const typeofAction = actionTypeValidator(list(String));

export function action (fullPath) {
    typeofSelectSite(...arguments);
    return {
        type: "ACTION_TYPE",
        payload: fullPath
    };
}

// Somewhere in your code
action(["some", "string", "here"]); // not throw

action("some"); // throw


```
