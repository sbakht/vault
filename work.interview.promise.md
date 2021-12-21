---
id: f7344bdb-ff3a-4a9d-88c9-43d5e3e88532
title: Promise
desc: ''
updated: 1640111100036
created: 1640111065205
---

Promise.resolve(5) 

const add = (x, y) => x + y
const increment = x => add(x, 1)
const decrement = x => add(x, -1)
 
Promise.resolve(5).then(x => {
	return add(x, 1)
}) 

Promise.resolve(5).then(increment) 

Promise.resolve(5).then(increment).then(increment) 

Promise.reject('error')

Promise.reject('error').then(increment).catch(x => console.log(x)) 

Promise.reject(5).then(increment).catch(decrement).then(decrement)

const randomPromise = new Promise((resolve, reject) => {
	setTimeout(() => {
		const random = Math.random();
		if(random > .5) {
			resolve(5)
		}else{
			reject(5)
		}
	}, 1000)
}).then(increment).catch(decrement) 

Promise.all([Promise.resolve(5), randomPromise]).then(x => console.log(x)) 

Promise.all([Promise.resolve(5), randomPromise]).then(x => console.log(x))



const get = async (url) => {
  if (!url) {
    throw new Error(`apiCLient get(): url attr is required, url: ${url}`);
  }

  let results;

  try {
    results = await $http.get(url);
  } catch (error) {
    throw new Error(`apiCLient get(): ${error}`);
  }

  if (!results.data) {
    throw new Error('apiCLient get(): results.data is empty');
  }

  return results.data;
};

