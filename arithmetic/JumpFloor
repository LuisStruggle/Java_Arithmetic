public class Solution
{
    /**
     * 一只青蛙一次可以跳上1级台阶，也可以跳上2级。求该青蛙跳上一个n级的台阶总共有多少种跳法
     * 思路，斐波那契数( 1:1, 2:2, 3:3, 4:5, 5:8, 6:13, 7:21 )
     * 
     * @param target
     * @return
     */
    private int JumpFloor(int target)
    {
        // 总跳法
        int sum = 0;

        int one = 1;
        int two = 2;

        if (target == 1)
        {
            sum = one;
        }
        else if (target == 2)
        {
            sum = two;
        }

        for (int i = 2; i < target; i++)
        {

            sum = one + two;
            one = two;
            two = sum;
        }

        return sum;
    }

    public static void main(String[] args)
    {
        Solution s = new Solution();

        System.out.println(s.JumpFloor(29));
    }

}
