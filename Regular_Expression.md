# Regular Expressions

10 minutes to manipulate regular expressions.

recommended regular expression test website:

> http://regex101.com

regular expression in many language:

> http://tool.rbtree.cn



## Grammar

### Single character repeat

`?`  0 or 1

```
read?

for

read
rea
```

`*` 0 or more

```
ab*c

for

ac
abc
abbc
abbbbc
```

`+` 1 or more

```
ab+c

for

abc
abbc
abbbc
```

`{number}` times it appears

```
ab{4}c

for

abbbbc
```

`{2,4}` appear 2-4 times

`{2,}` appear 2+ times

### Multiple character repeat

`(chars)` match multiple characters

```
(ab)+

for

ab
abab
ababab
```

### operators

#### Or

`|`

```
a (cat|dog)

for

a cat
a dog
```

#### not

`^`

```
[^0-9]+

for (all but numbers, including 换行符s)

dog
hello
```



`[chars]` characters taken from the dictionary

```
[abc]+

for 

abc

aabbcc
```

#### wildcard 通配符

a-z

A-Z

0-9

```
[a-zA-Z]+

for

tiger
abc
dog
ABCDEFG
```



#### 元字符 meta-characters

`\d`	numbers = [0-9]

`\D`	not numbers

`\w`	letters, numbers, and underscore

`\W`	not letters, numbers, and underscore

`\s`	blank space (including Tab and 换行符line break)

`\S`	not blank space

 `.` any character (not including 换行符) （要匹配句点使用 `\.`）

`\b` 单词的边界

#### match

`^` match top of line

`$` match end of line

```
^a

for

absorb
```

```
a$

for

tea
```

#### Greedy and lazy match 贪婪与懒惰匹配

默认情况下表达式会匹配尽可能多的字符

```
<.+>

<span>what <b>

会匹配整行
```

 将贪婪匹配转换为懒惰匹配

```
<.+?> //在加号右边加个问号
```

![image-20220604222323407](https://cdn.jsdelivr.net/gh/AppleisTasty/PicGarage/tmp/202206042223123.png)

![image-20220604222343003](https://cdn.jsdelivr.net/gh/AppleisTasty/PicGarage/tmp/202206042223175.png)



























