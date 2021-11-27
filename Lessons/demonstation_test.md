```js
// lib.spec.js

const { mapObjectToArray, getNewUser } = require('./myLib')

describe('mapObjectToArray', () => {
  test('maps arrays to values using callback', () => {
    const result = mapObjectToArray({age:30,height:65},(k,v)=>{
        return v+10
    })

    expect(result).toEqual([40,75])
  })

  test('callback gets called for each value', () => {
    const mockCb = jest.fn()

    mapObjectToArray({ a: 1, b: 1, c: 1 }, mockCb)
    expect(mockCb.mock.calls.length).toBe(3)
  })
})
```

# Navigation Link
- [Back](./tests.md)