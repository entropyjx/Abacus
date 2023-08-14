## Binary Search
```
//Compare with begin <= end
public int binarySearch(int[] nums, target) {
    int begin = 0;
    int end = nums.length - 1;
    while(begin <= end) {
        int mid = begin+end/2;
        if(target = nums[mid])
            return mid;
        if(target < nums[mid])
            end = mid - 1;
        else
            begin = mid + 1;
    }
    return -1;
}
```