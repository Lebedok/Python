# Python
First Unique Character in a String  Solution

Given a string, find the first non-repeating character in it and return it's index. If it doesn't exist, return -1.
s = "leetcode"
return 0.

s = "loveleetcode",
return 2.



class Solution(object):
    def firstUniqChar(self, s):
        word = s
        count = collections.Counter(s)
        
        for index, char in enumerate(s):
            if count[char] == 1:
                return index     
         
        return -1
  
