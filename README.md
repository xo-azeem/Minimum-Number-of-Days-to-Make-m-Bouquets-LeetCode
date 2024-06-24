# Minimum Number of Days to Make m Bouquets

LeetCode Q # 1482.

You are given an integer array bloomDay, an integer m and an integer k.</br>
You want to make m bouquets. To make a bouquet, you need to use k adjacent flowers from the garden.</br>
The garden consists of n flowers, the ith flower will bloom in the bloomDay[i] and then can be used in exactly one bouquet.</br>
Return the minimum number of days you need to wait to be able to make m bouquets from the garden. If it is impossible to make m bouquets return -1.</br>

Example 1:

>Input: bloomDay = [1,10,3,10,2], m = 3, k = 1</br>
>Output: 3</br>
>Explanation: Let us see what happened in the first three days. x means flower bloomed and _ means flower did not bloom in the garden.</br>
>We need 3 bouquets each should contain 1 flower.</br>
>After day 1: [x, _, _, _, _]   // we can only make one bouquet.</br>
>After day 2: [x, _, _, _, x]   // we can only make two bouquets.</br>
>After day 3: [x, _, x, _, x]   // we can make 3 bouquets. The answer is 3.</br>

Example 2:

>Input: bloomDay = [1,10,3,10,2], m = 3, k = 2</br>
>Output: -1</br>
>Explanation: We need 3 bouquets each has 2 flowers, that means we need 6 flowers. We only have 5 flowers so it is impossible to get the needed bouquets and we return -1.

Example 3:

>Input: bloomDay = [7,7,7,7,12,7,7], m = 2, k = 3</br>
>Output: 12</br>
>Explanation: We need 2 bouquets each should have 3 flowers.</br>
>Here is the garden after the 7 and 12 days:</br>
>After day 7: [x, x, x, x, _, x, x]</br>
>We can make one bouquet of the first three flowers that bloomed. We cannot make another bouquet from the last three flowers that bloomed because they are not adjacent.</br>
>After day 12: [x, x, x, x, x, x, x]</br>
>It is obvious that we can make two bouquets in different ways.</br>

My Solution Analysis:

<div align = "center">

  ![image](https://github.com/xo-azeem/Minimum-Number-of-Days-to-Make-m-Bouquets-LeetCode/assets/171427226/49250d89-2c79-414d-af5d-ed1fc7cb8dc5)

  Time complexity: O(log(max(bloomDay)) * n).</br>Space complexity: O(1).
</div>
