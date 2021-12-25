---
id: K0F1Cz3pTWOsHEHulMKwW
title: '121311'
desc: ''
updated: 1640011816486
created: 1639937593045
---

https://jsonplaceholder.typicode.com/guide/

const myPromiseAll = arr => {
  const result = []
  let count = 0;
  return new Promise((resolve, reject) => {
    arr.forEach((promise, i) => {
      if(!promise.then) {
        result[i] = promise 
        count++
        if(count === arr.length) {
          resolve(result)
        }
        return
      }
      promise.then(x =>  {
        result[i] = x
        count++
        if(count === arr.length) {
          resolve(result)
        }
      }).catch(reject)
    })
  })
}

const promise1 = Promise.resolve(3);
const promise2 = Promise.resolve(42);
const promise3 = new Promise((resolve, reject) => {
  setTimeout(resolve, 100, 'foo');
});
const promise4 = 5;
const rejected = Promise.reject("error message")

Promise.all([promise1, promise2, promise3, promise4]).then((values) => {
  console.log(values);
});

Promise.all([rejected, promise3]).then((values) => {
  console.log(values);
}).catch(err => {
  console.log(err)
})

myPromiseAll([promise1, promise2, promise3, promise4]).then((values) => {
  console.log(values);
});

myPromiseAll([rejected, promise3]).then((values) => {
  console.log(values);
}).catch(err => {
  console.log(err)
})

// Given an array of post ids, request those posts from the api, make the title uppercase and add an exclamation point, then send a request to update the titles in the api
// Once all the titles are successfully updated, log a success message

// write your own implementation of map
// write your own implementation of reduce