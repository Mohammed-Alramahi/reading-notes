# Node Ecosystem, TDD, CI/CD

---

1.map takes a callback function creating a new array after manipulating certain items from another array.

2.The reduce method executes a provided function for each value of the array (from left-to-right). The return value of the function is stored in an accumulator which hold the total.

3.Superagent example:

```javascript
const superAgent = require("superagent"); //after installing it through npm
superAgent.get(url).then((result) => console.log(result.body));
```

```javascript
const superAgent = require("superagent"); //after installing it through npm
const getData = async () => {
  let result = await superAgent.get(url);
};
```

4.We use promises in javascript because we sometimes need to get data from servers and javascript like any other language works synchronously and promises gives us the ability to do our intending job after getting the data back and same thing works with (async await).

5.Yes, because it depends on the data coming from that function that called the callback.
