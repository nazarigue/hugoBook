---
title: 'RegEx ✅'
date: 2019-02-11T19:27:37+10:00
draft: false
weight: 2
---


# Understanding RegEx

RegEx means regular expressions. It find patterns in your data.

|expression|purpose|
|---|---|
|`\d`|matches any digit|
|`\D`|matches any non-digit|
|`\w`|matches any word character (a-z, A-Z, 0-9, _)|
|`\W`|matches any non-word character|
|`\s`|matches any white space character (\r (carriage return),\n (new line), \t (tab), \f (form feed))|
|`\S`|matches any non-white space character|


|expression|purpose|
|---|---|
|`h.llo`| the "." matches any one character other than a new line character... matches "hello", "hallo" but not "h\nllo"|
|`h.*llo`|the "*" matches any character(s) zero or more times... matches "hello", "heeeeeello", "hllo", "hwarwareallo"|


|expression|purpose|
|---|---|
|`[a-z]`| matches all lowercase letters|
|`[A-Z]`| matches all uppercase letters|
|`[e-l]`| matches lowercase letters e to l (inclusive)|
|`[F-P]`| matches all uppercase letters F to P (inclusive)|
|`[0-9]`| matches all digits|
|`[5-9]`| matches any digit from 5 to 9 (inclusive)|
|`[a-zA-Z]`|matches all lowercase and uppercase letters|
|`[^a-zA-Z]`|matches non-letters|



[You can find full RegEx list here](https://gist.github.com/sarthology/b269c4ab81832c03f80eb48920f1abce "RegEx Regerence")