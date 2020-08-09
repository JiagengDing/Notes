---
title: "Doc" 
author: "Djg"
date: ""
output:
word_document:
toc: ture
# reference_doc: demo.docx
	
toc:
depth_from: 2
depth_to: 4
ordered: false
	
---

# Notes of Bash

## Variable

### echo

```bash {cmd = true}
ur_name="djg_laptop"
echo "${ur_name}Hi"
```

### unset

```bash {cmd = true}
ur_name="hi"
unset ur_name
echo "$ur_name"
echo '$ur_name'
```

### subStr

```bash {cmd = true}
str="abcd"
# length of str
echo ${#str}
echo ${str:1:2}
# find a or c
echo `expr index "$str" ac`
```

## List

```bash {cmd = true}
array=(v1 v2 v3)
array[3]=v4
echo ${array[@]}
```

```bash {cmd = true}
array=(v1 v2 v3)
echo ${#array[@]}
echo ${#array[*]}

echo ${#array[1]}
```

