# @kravc/request

No dependencies, simple, plain node.js helpers to execute HTTP and JSON
requests.

## API

Install:

```sh
npm i --save @kravc/request
```

### Get started

```js
const { jsonRequest } = require('@kravc/request')

const url = 'https://example.com/source.json'
const { object } = await jsonRequest(console, { url })
```

`object` is parsed response JSON body.

```js
const { httpRequest } = require('@kravc/request')

const url = 'https://example.com/source.html'
const { body: buffer } = await jsonRequest(console, { url })
```

`buffer` is raw response body.
