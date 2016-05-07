# Amelisa Redis

Redis pubsub for [Amelisa](https://github.com/amelisa/amelisa)

[![js-standard-style](https://cdn.rawgit.com/feross/standard/master/badge.svg)](https://github.com/feross/standard)

### Features

- Redis pubsub (for horizontal scaling)
- Memory pubsub (for tests)

### Installation

```
$ npm install amelisa-redis
```

### Usage

```js
import RedisPubsub from 'amelisa-redis/RedisPubsub'

let pubsub = new RedisPubsub(process.env.REDIS_URL)
let store = new Store({pubsub})
```

or for memory pubsub

```js
import MemoryPubsub from 'amelisa-redis/MemoryPubsub'

let pubsub = new MemoryPubsub()
let store = new Store({pubsub})
```

### Example
- [amelisa-crud-example](https://github.com/amelisa/amelisa-crud-example) example app with auth

### MIT License
Copyright (c) 2016 by Vladimir Makhaev

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
