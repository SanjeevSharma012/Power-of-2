##Check if a Number is Power of Two in Java
📌 Problem Statement

Given an integer n, determine whether it is a power of 2.

##💡 Approach
A power of 2 has only one set bit (1) in its binary representation.
Subtracting 1 from such a number flips all bits after that set bit.
Performing a bitwise AND between n and n - 1 results in 0 only if n is a power of 2.
Handle edge cases like n <= 0.
---

##🧾Code
class Solution {
    public static boolean isPowerofTwo(int n) {
        if (n <= 0) return false;
        return (n & (n - 1)) == 0;
    }
}
📥 Input

An integer n

📤 Output

Boolean value:

true → if n is a power of 2
false → otherwise
🧪 Example
Input
n = 4
Output
true
Input
n = 6
Output
false
---
⚠️ Note
0 and negative numbers are not powers of 2.
This solution uses an efficient bit manipulation technique with O(1) time complexity.
✍️ Author

Sanjeev Sharma
