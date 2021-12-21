---
id: 374c73e8-ee8f-4197-a966-e68df5b454de
title: Es6
desc: ''
updated: 1640111149402
created: 1640111137554
---

const arr1 = [1,2,3]
arr1.push(4)
arr1 = [1,2,3,4,5]

let arr2 = [1,2,3]
arr2.push(4)
arr2 = [1,2,3,4,5]

function getNumber(bool) {
	if(bool) {
		let result = 5;
	}else{
		let result = 10;
	}
	return result;
}

const Animal1 = {
	name: 'Cat',
	speak() {
		console.log(`I am a ${this.name}`)
	}
}

Animal1.speak();

const Animal2 = {
	name: 'Cat',
	speak: () => {
		console.log(`I am a ${this.name}`)
	}
}

Animal2.speak()

const add2 = (x = 1, y = 2) => {
	return x + y;
}

add2(3)

const obj = {foo: "a", bar: "b", baz: "c"}

const { foo, baz } = obj

const obj2 = {...obj, alpha: 'd'}

obj2.foo = "new foo"

const obj3 = {...obj, ...obj2}

obj2 === obj3