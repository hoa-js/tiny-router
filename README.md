## @hoajs/tiny-router

Tiny router middleware for Hoa.

## Installation

```bash
$ npm i @hoajs/tiny-router --save
```

## Quick Start

```js
import { Hoa } from 'hoa'
import { tinyRouter } from '@hoajs/tiny-router'

const app = new Hoa()
app.extend(tinyRouter())

app.get('/users/:name', async (ctx, next) => {
  ctx.res.body = `Hello, ${ctx.req.params.name}!`
})

export default app
```

## Documentation

The documentation is available on [hoa-js.com](https://hoa-js.com/middleware/router/tiny-router.html)

## Test (100% coverage)

```sh
$ npm test
```

## License

MIT
