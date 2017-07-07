---
layout: post
title: Inverted Index 五分钟教程
date: 2017-07-07 10:00:00.000000000 +08:00
tags: inverted-index index druid
---

## Example
### Example1: search on Docs
Doc A:
> The quick brown fox jumped over the lazy dog

Doc B:
> Quick brown foxes leap over lazy dogs in summer

result:

Term    |  Doc_1 | Doc_2
-------- | ------ | ----
Quick   |       |  X
The     |   X   |
brown   |   X   |  X
dog     |   X   |
dogs    |       |  X
fox     |   X   |
foxes   |       |  X
in      |       |  X
jumped  |   X   |
lazy    |   X   |  X
leap    |       |  X
over    |   X   |  X
quick   |   X   |
summer  |       |  X
the  |X   |

A good example:
![index in textbook](https://qph.ec.quoracdn.net/main-qimg-313e47647edc7807f827127b7811b441)

### Example2: index in druid
see:
[druid segments](http://druid.io/docs/0.9.2/design/segments.html#multi-value-columns)
