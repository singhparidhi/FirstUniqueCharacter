import java.util.HashMap;

public class Solution {
    public int firstUniqChar(String s) {
        // Step 1: Initialize hashmap to store character frequencies
        HashMap<Character, Integer> freqMap = new HashMap<>();

        // Step 2: Update character frequencies in hashmap
        for (int i = 0; i < s.length(); i++) {
            char c = s.charAt(i);
            freqMap.put(c, freqMap.getOrDefault(c, 0) + 1);
        }

        // Step 3: Find the first non-repeating character and return its index
        for (int i = 0; i < s.length(); i++) {
            char c = s.charAt(i);
            if (freqMap.get(c) == 1) {
                return i;
            }
        }

        // Step 4: No non-repeating character found
        return -1;
    }

    public static void main(String[] args) {
        Solution solution = new Solution();

        String s1 = "leetcode";
        int index1 = solution.firstUniqChar(s1);
        System.out.println(index1);  // Output: 0

        String s2 = "loveleetcode";
        int index2 = solution.firstUniqChar(s2);
        System.out.println(index2);  // Output: 2

        String s3 = "aabb";
        int index3 = solution.firstUniqChar(s3);
        System.out.println(index3);  // Output: -1
    }
}
