# Vitest

Vitest is a kind of test runner. Test Runner is 測試執行器. There are some common test runner, such as:
1. Jest
2. Cypress
3. WebdriverIO
4. Web Test Runner
5. uvu

Question: Vitest and Jest, are test runners, and are also testing frameworks?

My understanding through the descriptions on vitest.dev/guide/comparisions.html:

## Jest v.s. Vitest

- Jest has the feature called `it` and `expect`, and `it` and `expect` are APIs.
- Most software testing needs `snapshtos`, `nocks` and `coverage`, and Jest has a full pack of it.
- Vitest offers compatibility with most of the Jest API.
- What does it mean `Jest ecosystem libraries`? Ecosystem?

## Cypress v.s. Vitest

Cypress is a browser-based test runner.
Cypress is known as an end-to-end testing tool.

Question: What does `end-to-end testing tool` mean?

## API

### Test API Reference
### Mock Functions
### Vi Utility
### Expect
### ExpectTypeOf
### Assert

Q: assert is like boolean?

#### assert

```ts
import { assert, test } from 'vitest';

test('assert', () => {
  assert('foo' !== 'bar', 'food should not be equal to bar.');
});
```

#### fail

Type:
- (message?: string) => never
- 

Explanation:
- (message?: string)
  It means that the message as the parameter is optional to be a string.
- => never
  It means that the function should never successfully return a value.

```ts
import { assert, test} from 'vitest';

test('assert.fail', () => {
  assert.fail('error message on failure');
  assert.fail('foo', 'bar', 'foo is not bar', '===');
});
```

### AssertType


