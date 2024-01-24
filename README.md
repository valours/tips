# tricks--t-j-s
## Affectation
```typescript
// Before
let name = '';
if (!name) {
  name = 'name';
}

// After
let name = '';
name =|| 'name';
```
## Null or undefined
```typescript
// Before
let result;
if (variable !== null && variable !== undefined) {
  result = variable;
} else {
  result = 'Default';
}

// After
const result = variable ?? 'Default';
```
## Ensuring Unique Elements
```typescript
// Before
const numbers = [1,2,3,3];
const uniqueNumbers = Array.from(new Set(numbers));

// After
const numbers = [1,2,3,3];
const uniqueNumbers = [...new Set(numbers)];
```
## Toggling Boolean
```typescript
// Before
let isActive = true;
isActive = !Active;

// After
let isActive = true;
isActive ^= isActive;
``` 

