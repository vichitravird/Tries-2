# Tries-2

## Problem1: List of word squares(https://leetcode.com/problems/word-squares/)
From a given set of words, find all the word squares you can build from them.

A sequence of words forms a valid word square if the kth row and column read the exact same string, where 0 ≤ k < max(numRows, numColumns).

For example, the word sequence ["ball","area","lead","lady"] forms a word square because each word reads the same both horizontally and vertically.

b a l l

a r e a

l e a d

l a d y

Note:

There are at least 1 and at most 1000 words.

Example 1:

Input:

["area","lead","wall","lady","ball"]

Output:

[
 
 [ "wall",
 
 "area",
 
 "lead",
 
 "lady"
 
 ],
 
 [ "ball",
 
 "area",
 
 "lead",
 
 "lady"
 
 ]

]


Explanation:

The output consists of two word squares. The order of output does not matter (just the order of words in each word square matters).

Example 2:

Input:

["abat","baba","atan","atal"]

Output:

[

 [ "baba",

"abat",

"baba",

"atan"

],

[ "baba",

"abat",

"baba",

"atal"

]

]

Explanation:

The output consists of two word squares. The order of output does not matter (just the order of words in each word square matters).

## Problem2: Match Camelcases(https://leetcode.com/problems/camelcase-matching/)

A query word matches a given pattern if we can insert lowercase letters to the pattern word so that it equals the query. (We may insert each character at any position, and may insert 0 characters.)

Given a list of queries, and a pattern, return an answer list of booleans, where answer[i] is true if and only if queries[i] matches the pattern.

Example 1:

Input: queries = ["FooBar","FooBarTest","FootBall","FrameBuffer","ForceFeedBack"], pattern = "FB"

Output: [true,false,true,true,false]

Explanation: 

"FooBar" can be generated like this "F" + "oo" + "B" + "ar".

"FootBall" can be generated like this "F" + "oot" + "B" + "all".

"FrameBuffer" can be generated like this "F" + "rame" + "B" + "uffer".

Example 2:

Input: queries = ["FooBar","FooBarTest","FootBall","FrameBuffer","ForceFeedBack"], pattern = "FoBa"

Output: [true,false,true,false,false]

Explanation: 

"FooBar" can be generated like this "Fo" + "o" + "Ba" + "r".

"FootBall" can be generated like this "Fo" + "ot" + "Ba" + "ll".

Example 3:

Input: queries = ["FooBar","FooBarTest","FootBall","FrameBuffer","ForceFeedBack"], pattern = "FoBaT"

Output: [false,true,false,false,false]

Explanation: 

"FooBarTest" can be generated like this "Fo" + "o" + "Ba" + "r" + "T" + "est".

Note:

1 <= queries.length <= 100

1 <= queries[i].length <= 100

1 <= pattern.length <= 100

All strings consists only of lower and upper case English letters.

