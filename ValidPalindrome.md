
Problem Link: https://leetcode.com/problems/valid-palindrome/
```
class Solution {
    public boolean isPalindrome(String s) {
        
        String s1 = s.toLowerCase().replaceAll("[^a-zA-Z0-9]", "");
        
        StringBuilder sb = new StringBuilder();
        
        sb.append(s1);
        
        String s2 = sb.reverse().toString();
        
        if(s1.equals(s2)) return true;
        else return false;
        
    }
    
}
```
