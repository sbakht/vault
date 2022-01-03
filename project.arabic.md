---
id: 1f739aa3-9a4c-4a93-96e7-4a8867a5ac7c
title: Arabic
desc: ''
updated: 1641062251111
created: 1637198980521
---

## Random notes for the arabic project

### Sarf stuff

pick the sarf pattern multiple choice question. Data for each word will have entry key for associated pattern
pattern
{
	id: 1,
	displayName: 'akarama'
}
{
	roots: [4, 3, 5] // each letter will have an id to associate root letters this way
	displayName: 'afala',
	pattern: 1
}


### Resouraces

https://ctan.org/pkg/arabtex?lang=en - latex arabic
https://kariminf.github.io/jslingua.web/trans.html - transliteration
https://github.com/purescript-contrib/purescript-unicode - unicode for arabic characters
http://www.qamus.org/transliteration.htm
https://corpus.quran.com/java/buckwalter.jsp

![[arabic.bayyinah.day73#What-to-do-when-you-see-a-fil-in-Quran]]

process to building passive verb - https://dream.bayyinahtv.com/topics/41/session/215/video/2316

## Verb interactive teacher

![](/assets/images/2021-12-25-11-42-12.png)

*Steps to create arabic negation from english*

**Neither of you will go**

1. Identify the verb
2. Translate the verb to basic form
3. Get right tense of verb (there is a problem here cause the harf can change you to use present when using lam)
3. Get the right form of verb from gender and plurality
4. Identify any harf needed for meaning
5. Modify verb if needed by the harf
	- go back to step 3 if needed


### Options for question types

single choice - single direction

multiple choice with single select (or other variates of fixed selection)
	- single flow
	- each own direction
	- right/wrong direction

multiple choice with multi select (or other variations of fixed selection)
	- single flow
	- each combination own direction or closed set of directions
	- right/wrong direction

user inputed string
	- single direction
	- parse and switch case into multiple directions

user string + multiple choies