class Solution {
    public int maximumCount(int[] nums) {
        int negCount = 0;
        int posCount = 0;
        
        for (int num : nums) {
            if (num < 0) {
                negCount++;
            } else if (num > 0) {
                posCount++;
            }
            // Skip zero as it's neither positive nor negative
        }
        
        return Math.max(negCount, posCount);
    }
}
