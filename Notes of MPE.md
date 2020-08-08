---
title: "Doc"
author: "Djg"
date: "2020-08-07"
output:
    word_document:
        toc: ture
        # reference_doc: demo.docx

toc:
  depth_from: 2
  depth_to: 4
  ordered: false

  presentation:
  width: 1080
  height: 720
---

# Markdown Notes

[TOC]

| Column A | Column B | Column C |
| -------- | -------- | -------- |
| A1       | B1       | C1       |
| A2       | B2       | C2       |
| A3       | B3       | C3       |

| aa  | rr  | ss  | tt  | dd  |
| --- | --- | --- | --- | --- |
| aa  | rr  | ss  | tt  | dd  |
| aa  | rr  | ss  | tt  | dd  |
| aa  | rr  | ss  | tt  | dd  |

H~2~O
20^th^

content [^1]

<!-- [^1]: This is content! -->

==marked==

$$\sqrt{2500} = 50$$

## This is Ditaa

```ditaa {cmd=true args=["-E"]}
+--------+             +----------+
|        |    5mins    |          |
| My Home|------------>| ZC's Home|
|     {d}|             |          |
+---+----+             +-----+----+
    :                        ^
    |           bikes        |
    +------------------------+
```

## Import File

@import "test.jl"

@import "test.jl" {code_block=true class="line-numbers" cmd="julia"}

@import "test.jl" {as="vega-lite"}

```javascript {cmd="node"}
const date = Date.now()
console.log(date.toString())
```

## Slides

cmd+shift+p
Slides

## Code Chunk

```bash {cmd=true}
ls .
```

## Macro

### Matplotlib

```python {cmd=true matplotlib=true}
import matplotlib.pyplot as plt
plt.plot([1,2,3, 4])
plt.show() # show figure
```
