# Enforce the use of `Buffer.from()` and `Buffer.alloc()` instead of the deprecated `new Buffer()`

<!-- Do not manually modify RULE_NOTICE part. Run: `npm run generate-rule-notices` -->
<!-- RULE_NOTICE -->
✅ *This rule is part of the [recommended](https://github.com/sindresorhus/eslint-plugin-unicorn#recommended-config) config.*

🔧💡 *This rule is [auto-fixable](https://eslint.org/docs/user-guide/command-line-interface#fixing-problems) and provides [suggestions](https://eslint.org/docs/developer-guide/working-with-rules#providing-suggestions).*
<!-- /RULE_NOTICE -->

Enforces the use of [Buffer.from](https://nodejs.org/api/buffer.html#static-method-bufferfromarray) and [Buffer.alloc()](https://nodejs.org/api/buffer.html#static-method-bufferallocsize-fill-encoding) instead of [new Buffer()](https://nodejs.org/api/buffer.html#new-bufferarray), which has been deprecated since Node.js 4.

## Fail

```js
const buffer = new Buffer('7468697320697320612074c3a97374', 'hex');
```

```js
const buffer = new Buffer([0x62, 0x75, 0x66, 0x66, 0x65, 0x72]);
```

```js
const buffer = new Buffer(10);
```

## Pass

```js
const buffer = Buffer.from('7468697320697320612074c3a97374', 'hex');
```

```js
const buffer = Buffer.from([0x62, 0x75, 0x66, 0x66, 0x65, 0x72])
```

```js
const buffer = Buffer.alloc(10);
```
