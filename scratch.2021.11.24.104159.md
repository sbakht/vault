---
id: 81e26014-abba-4a83-9625-54725eb5f90e
title: '104159'
desc: ''
updated: 1637773385313
created: 1637772119990
---

page loads with no params -> load default params
page loads with params -> use those instead of default in the api request
do not update url on ssr request

user does interaction -> update url on api rquest

url changes without request (back button) -> trigger request