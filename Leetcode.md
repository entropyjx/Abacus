## 34. Find First and Last Position of Element in Sorted Array

* https://leetcode.com/problems/find-first-and-last-position-of-element-in-sorted-array/

### Notes:
Use Binary Search to find the target, then test if it's the first or last element by checking the element to the left or right, and if it's at begin or end.

## 7. Reverse Integer

* https://leetcode.com/problems/reverse-integer/

### Notes:
Mod by 10, divide by 10, and for result, multiply by 10.

```
    public int reverse(int x) {
        int sum = 0;
        while(x!=0) {
            int digit = x % 10;
            if(sum>Integer.MAX_VALUE / 10 || sum < Integer.MIN_VALUE / 10)
                return 0;
            sum = sum * 10 + digit;
            x/=10;
        }
        return (int) sum;
    }
```