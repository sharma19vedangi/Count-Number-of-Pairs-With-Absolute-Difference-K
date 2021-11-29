# Count-Number-of-Pairs-With-Absolute-Difference-K
#Array Leetcode Problem Solution
class Solution {
    public int countKDifference(int[] nums, int k) {
        int len = nums.length, count = 0;
        for(int i=0; i<len; i++){
            for(int  j=i; j<len; j++){
                int n = nums[i]-nums[j];
                if(Math.abs(n) == k){
                    count++;
                }
            }
        }
        return count;
    }
}
