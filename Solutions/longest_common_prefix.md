# null

**Difficulty:** Easy

**LeetCode:** [Link](https://leetcode.com/problems/longest-common-prefix/)

## Description
Write a function to find the longest common prefix string amongst an array of strings.

If there is no common prefix, return an empty string "".

 
Example 1:

Input: strs = ["flower","flow","flight"]
Output: "fl"


Example 2:

Input: strs = ["dog","racecar","car"]
Output: ""
Explanation: There is no common prefix among the input strings.


 
Constraints:


	1 <= strs.length <= 200
	0 <= strs[i].length <= 200
	strs[i] consists of only lowercase English letters if it is non-empty.

## Solution
```
            int j = 0;            int j = 0;
            while (j < prefix.size() && j < strs[i].size() &&            while (j < prefix.size() && j < strs[i].size() &&
                   prefix[j] == strs[i][j]) {                   prefix[j] == strs[i][j]) {
                j++;                j++;
            }            }
            prefix = prefix.substr(0, j);            prefix = prefix.substr(0, j);
            if (prefix.empty()) return "";            if (prefix.empty()) return "";
        }        }

        string prefix = strs[0];        string prefix = strs[0];

        for (int i = 1; i < strs.size(); i++) {        for (int i = 1; i < strs.size(); i++) {
        if (strs.empty()) return "";        if (strs.empty()) return "";

class Solution {class Solution {
public:public:
    string longestCommonPrefix(vector<string>& strs) {    string longestCommonPrefix(vector<string>& strs) {
```

---
*Last updated: 2026-01-09T09:58:12.972Z*
