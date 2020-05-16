```js
const items = [{id: 1}, {id: 2}, {id: 3}];
```

## Add new item at the start (`unshift`)
```js
let item = {id: 0};
items.unshift(item);
```

## Add new item at the end (`push`)
```js
let item = {id: 5};
items.push(item);
```

## Add new item in the middle (`splice`)
```js
let item = {id: 4};
// Array.splice({index where to start}, {how many items to remove}, {items to add});
items.splice(4, 0, item);
```

## Find an item in an array by its values (`find`)
```js
let result = items.find(x => x.id === 2);
```

## Get multiple items from an array that match a condition (`filter`)
```js
let result = items.filter(x => x.id % 2);
```

## Transform items of an array (`map`)
```js
let result = items.map(x => x.id);
```

## Add a property to every item of an array (`forEach`)
```js
items.forEach((x, i) => x['index']= i + 1);
```

## Sort an array by a property (`sort`)
```js
items.sort((a, b) => a.id < b.id);
```

## Check each item for a specific condition (`every`, `some`)
```js
let result = items.some(x => x.id === 2); // true
let result = items.every(x => x.id === 2); // false
```
