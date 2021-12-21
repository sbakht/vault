---
id: b52d2eac-33d5-4095-8c5c-93489c522fd0
title: Recursion
desc: ''
updated: 1640111173601
created: 1640111167137
---

function fibonacci(num) {
	if(num < 2) {
			return num;
	}
	else {
			return fibonacci(num-1) + fibonacci(num - 2);
	}
}