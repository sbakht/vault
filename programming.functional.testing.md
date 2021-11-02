---
id: W3MsgkUALhXOPECilKaPt
title: Testing
desc: ''
updated: 1635821635728
created: 1635821624430
---

## Benefits of functional composition in respects to unit testing

https://medium.com/javascript-scene/mocking-is-a-code-smell-944a70c90a6a

1. Pub/sub to decouple IO from logic
2. composition functions that return promises
3. Future compositions (we can't really do this i think)

### Pub Sub

Store dispatch is a pub sub. I can make a pub sub between the ajax request and fake a response event with the fake ajax data response.
