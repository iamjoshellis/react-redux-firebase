<!-- Generated by documentation.js. Update this documentation by updating the source code. -->

# actionsPrefix

Prefix for all actions within library

**Examples**

```javascript
import { constants } from 'react-redux-firebase'
constants.actionsPrefix === '@@reactReduxFirebase' // true
```

# actionTypes

Object containing all action types

**Properties**

-   `START` **[String](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)** `@@reactReduxFirebase/START`
-   `SET` **[String](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)** `@@reactReduxFirebase/SET`
-   `SET_PROFILE` **[String](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)** `@@reactReduxFirebase/SET_PROFILE`
-   `LOGIN` **[String](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)** `@@reactReduxFirebase/LOGIN`
-   `LOGOUT` **[String](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)** `@@reactReduxFirebase/LOGOUT`
-   `LOGIN_ERROR` **[String](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)** `@@reactReduxFirebase/LOGIN_ERROR`
-   `NO_VALUE` **[String](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)** `@@reactReduxFirebase/NO_VALUE`
-   `UNAUTHORIZED_ERROR` **[String](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)** `@@reactReduxFirebase/UNAUTHORIZED_ERROR`
-   `INIT_BY_PATH` **[String](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)** `@@reactReduxFirebase/INIT_BY_PATH`
-   `AUTHENTICATION_INIT_STARTED` **[String](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)** `@@reactReduxFirebase/AUTHENTICATION_INIT_STARTED`
-   `AUTHENTICATION_INIT_FINISHED` **[String](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)** `@@reactReduxFirebase/AUTHENTICATION_INIT_FINISHED`
-   `FILE_UPLOAD_START` **[String](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)** `@@reactReduxFirebase/FILE_UPLOAD_START`
-   `FILE_UPLOAD_ERROR` **[String](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)** `@@reactReduxFirebase/FILE_UPLOAD_ERROR`
-   `FILE_UPLOAD_PROGRESS` **[String](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)** `@@reactReduxFirebase/FILE_UPLOAD_PROGRESS`
-   `FILE_UPLOAD_COMPLETE` **[String](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)** `@@reactReduxFirebase/FILE_UPLOAD_COMPLETE`
-   `FILE_DELETE_START` **[String](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)** `@@reactReduxFirebase/FILE_DELETE_START`
-   `FILE_DELETE_ERROR` **[String](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)** `@@reactReduxFirebase/FILE_DELETE_ERROR`
-   `FILE_DELETE_COMPLETE` **[String](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)** `@@reactReduxFirebase/FILE_DELETE_COMPLETE`

**Examples**

```javascript
import { actionTypes } from 'react-redux-firebase'
actionTypes.SET === '@@reactReduxFirebase/SET' // true
```

# defaultConfig

Default configuration options

**Properties**

-   `userProfile` **[String](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)** `null` Location on Firebase where user
    profiles are stored. Often set to `'users'`.
-   `enableLogging` **[Boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean)** `false` Whether or not firebase
    database logging is enabled.
-   `updateProfileOnLogin` **[Boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean)** `true` Whether or not to update
    user profile when logging in.
-   `enableRedirectHandling` **[Boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean)** `true` Whether or not to enable
    redirect handling. This must be disabled if environment is not http/https
    such as with react-native.
-   `autoPopulateProfile` **[Boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean)** `true` Whether or not to
    automatically populate profile with data loaded through
    profileParamsToPopulate config.
-   `setProfilePopulateResults` **[Boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean)** `true` Whether or not to
    call SET actions for data that results from populating profile to redux under
    the data path. For example: role paramter on profile populated from 'roles'
    root. True will call SET_PROFILE as well as a SET action with the role that
    is loaded (places it in data/roles).
