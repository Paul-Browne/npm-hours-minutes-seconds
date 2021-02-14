# npm-hours-minutes-seconds
constant width time eg. 12:34:56 or 03:02:01

### usage

`npm i hours-minutes-seconds`

or 

`npm i -D hours-minutes-seconds`

Called with no arguments, the time will be the current time.

```js
const hms = require('hours-minutes-seconds')
console.log(hms());  // 09:15:27 (if the time was quarter past nine in the morning)
```

Alternatively pass a date object.

```js
const hms = require('hours-minutes-seconds')
const timeIn30Minutes = new Date(+new Date() + 1.8e6);
console.log(hms(timeIn30Minutes));  // 09:45:27 (if the time was quarter past nine in the morning)
```