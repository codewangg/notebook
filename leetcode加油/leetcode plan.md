## 二分法

基本问题：

1. 基本思想？（有序的数据，每次通过判断逻辑排除掉一部分的答案，直到触发终止条件）
2. 二分法实现模板（可以递归，可以迭代；一般以迭代为主）
3. 移动两个指针（start与end）的含义？移动条件是什么（筛选掉一部分数据的依据）？循环的截止条件？
4. 数据中是否有重复数字？对结果有什么影响？
5. 为什么你选择的模板中使用start<end或者start<=end或者start+1<end作为终止条件？这样写是如何避免死循环的？不这么写在什么情况下会出现死循环？
6. 在处理逻辑中，当前结果><=目标值时分别如何处理？移动指针的依据是什么？
7. 循环退出后是否需要额外处理？
8. 如果遇到cornercase根本没进主循环，你的代码是否能正常工作？
9. 为什么Java需要写mid=start+(end-start)/2而Python可以直接写mid=(start+end)//2？
10. 如何理解从基本的朴素二分，到相对复杂的条件二分，到更加抽象的答案二分？（在一个显性有序数组中一次砍掉一部分-->在一组有规律的数据上利用判断条件逐步缩小范围-->在一个有序的抽象模型里，利用不断的"猜测+检验"逐步逼近最终结果）

### 朴素二分法

- [x] <span style='color:#9966ff;background:背景颜色;font-size:文字大小;'>704. BinarySearch </span>

- [x] <span style='color:#6699ff;background:背景颜色;font-size:文字大小;'>34. Find First and Last Position of Element in Sorted Array</span>
- [x] <span style='color:#6699ff;background:背景颜色;font-size:文字大小;'>702. Search in a Sorted Array of Unknown Size</span>
- [ ] <span style='color:#99CC66;background:背景颜色;font-size:文字大小;'>153.Find Minimum in Rotated Sorted Array</span>
- [ ] <span style='color:#99CC66;background:背景颜色;font-size:文字大小;'>154.Find Minimum in Rotated Sorted Array II</span>
- [ ] <span style='color:#99CC66;background:背景颜色;font-size:文字大小;'>278.First Bad Version</span>
- [ ] <span style='color:#99CC66;background:背景颜色;font-size:文字大小;'>658.Find K Closest Elements</span>

### 条件二分法

- [ ] <span style='color:#9966ff;background:背景颜色;font-size:文字大小;'>33. Search in Rotated Sorted Array</span>
- [ ] <span style='color:#9966ff;background:背景颜色;font-size:文字大小;'>81. Search in Rotated Sorted Array(2)</span>
- [ ] <span style='color:#6699ff;background:背景颜色;font-size:文字大小;'>4. Median of Two Sorted Arrays</span>
- [ ] <span style='color:#6699ff;background:背景颜色;font-size:文字大小;'>74. Search a 2D Matrix</span>
- [ ] <span style='color:#6699ff;background:背景颜色;font-size:文字大小;'>162.Find Peak Element</span>
- [ ] <span style='color:#99CC66;background:背景颜色;font-size:文字大小;'>302.Smallest Rectangle Enclosing Black Pixels</span>
- [ ] <span style='color:#99CC66;background:背景颜色;font-size:文字大小;'>852.Peak Index in a Mountain Array</span>

### 答案二分法

- [ ] <span style='color:#6699ff;background:背景颜色;font-size:文字大小;'>875.[Koko Eating Bananas](</span>

- [ ] <span style='color:#6699ff;background:背景颜色;font-size:文字大小;'>1283.[Find the Smallest Divisor Givena Threshold](</span>

- [ ] <span style='color:#99CC66;background:背景颜色;font-size:文字大小;'>69.Sqrt(x)</span>

- [ ] <span style='color:#99CC66;background:背景颜色;font-size:文字大小;'>Lint-586.Sqrt(x) II</span>

- [ ] <span style='color:#99CC66;background:背景颜色;font-size:文字大小;'>Lint-183.Wood Cut</span>

- [ ] <span style='color:#99CC66;background:背景颜色;font-size:文字大小;'>Lint-437.Copy Books</span>

- [ ] <span style='color:#99CC66;background:背景颜色;font-size:文字大小;'>Lint-438.Copy Books II</span>

  

## 多指针

基本问题：

1. 多指针是一个非常广泛的概念，并不是一个固定的算法。但基本上是通过一些变量的控制与循环把问题的复杂度控制在一两层for循环之内。可以用在数组、链表、区间、滑动窗口、流、回文串、和差问题等多个场景。（前项和其实并不完全是指针问题，但也归并在这里）。
2. QuickSort和MergeSort的基本原理与实现，排序的稳定性问题
3. QuickSelect的实现与复杂度
4. 同向指针与相向指针的使用场景
5. 不同场景下循环终止条件？
6. 两数之和，之差，特定条件下（大小于某值等）的计数问题
7. 三数或三数以上之和的通用写法（两数之和+搜索）
8. 数组有没有排序？是否需要排序？
9. 数组有没有去重？是否需要去重？
10. 离线数据（内存中，有限长）还是在线数据（无法放入内存，长度未知）？
11. 链表操作中dummynode与previousnode的使用技巧
12. 链表的中点，判断是否有环，寻找环的交叉点



### 数组

- [ ] <span style='color:#9966ff;background:背景颜色;font-size:文字大小;'>912.Sort an Array, Quick Sort and Merge Sort</span>
- [ ] <span style='color:#9966ff;background:背景颜色;font-size:文字大小;'>75.Sort Colors</span>
- [ ] <span style='color:#6699ff;background:背景颜色;font-size:文字大小;'>26.Remove Duplicates from Sorted Array</span>
- [ ] <span style='color:#6699ff;background:背景颜色;font-size:文字大小;'>80.Remove Duplicates from Sorted ArrayII</span>
- [ ] <span style='color:#6699ff;background:背景颜色;font-size:文字大小;'>88.Merge Sorted Array</span>
- [ ] <span style='color:#6699ff;background:背景颜色;font-size:文字大小;'>283.Move Zeroes</span>
- [ ] <span style='color:#6699ff;background:背景颜色;font-size:文字大小;'>215 K-th Largest Element in an Array</span>
- [ ] <span style='color:#6699ff;background:背景颜色;font-size:文字大小;'>347.Top K Frequent Elements</span>
- [ ] <span style='color:#6699ff;background:背景颜色;font-size:文字大小;'>349.Intersection of Two Arrays</span>
- [ ] <span style='color:#6699ff;background:背景颜色;font-size:文字大小;'>350 Intersection of Two ArraysII</span>
- [ ] <span style='color:#6699ff;background:背景颜色;font-size:文字大小;'>845.Longest Mountain in Array</span>
- [ ] <span style='color:#6699ff;background:背景颜色;font-size:文字大小;'>42.Trapping Rain Water</span>
- [ ] <span style='color:#6699ff;background:背景颜色;font-size:文字大小;'>43.Multiply Strings</span>
- [ ] <span style='color:#99CC66;background:背景颜色;font-size:文字大小;'>969.Pancake Sorting</span>
- [ ] <span style='color:#99CC66;background:背景颜色;font-size:文字大小;'>Lint-31.Partition Array</span>
- [ ] <span style='color:#99CC66;background:背景颜色;font-size:文字大小;'>Lint-625.Partition Array II</span>
- [ ] <span style='color:#99CC66;background:背景颜色;font-size:文字大小;'>Lint-143.Sort Color II</span>
- [ ] <span style='color:#99CC66;background:背景颜色;font-size:文字大小;'>Lint-461.Kth Smallest Numbers in Unsorted Array</span>
- [ ] <span style='color:#99CC66;background:背景颜色;font-size:文字大小;'>Lint-544.Top k Largest Numbers</span>

### 链表

- [ ] <span style='color:#9966ff;background:背景颜色;font-size:文字大小;'>21.Merge Two Sorted Lists</span>
- [ ] <span style='color:#6699ff;background:背景颜色;font-size:文字大小;'>86.Partition List</span>
- [ ] <span style='color:#6699ff;background:背景颜色;font-size:文字大小;'>141.Linked List Cycle</span>
- [ ] <span style='color:#6699ff;background:背景颜色;font-size:文字大小;'>160.Intersection of Two Linked Lists</span>
- [ ] <span style='color:#6699ff;background:背景颜色;font-size:文字大小;'>234.Palindrome LinkedList</span>
- [ ] <span style='color:#6699ff;background:背景颜色;font-size:文字大小;'>328.Odd Even LinkedList</span>
- [ ] <span style='color:#99CC66;background:背景颜色;font-size:文字大小;'>142.Linked List Cycle II</span>
- [ ] <span style='color:#99CC66;background:背景颜色;font-size:文字大小;'>287.Find the Duplicate Number</span>



### 区间

- [ ] <span style='color:#9966ff;background:背景颜色;font-size:文字大小;'>Lint-391.Number of Airplanes in the Sky</span>
- [ ] <span style='color:#6699ff;background:背景颜色;font-size:文字大小;'>56.Merge Intervals</span>
- [ ] <span style='color:#6699ff;background:背景颜色;font-size:文字大小;'>57.Insert Interval</span>
- [ ] <span style='color:#6699ff;background:背景颜色;font-size:文字大小;'>252.Meeting Rooms</span>
- [ ] <span style='color:#6699ff;background:背景颜色;font-size:文字大小;'>253.Meeting Rooms II</span>
- [ ] <span style='color:#6699ff;background:背景颜色;font-size:文字大小;'>986.Interval List Intersections</span>

### 回文串

- [ ] <span style='color:#6699ff;background:背景颜色;font-size:文字大小;'>5.Longest Palindromic Substring</span>

- [ ] <span style='color:#6699ff;background:背景颜色;font-size:文字大小;'>345.Reverse Vowels of a String</span>
- [ ] <span style='color:#6699ff;background:背景颜色;font-size:文字大小;'>680.Valid Palindrome II</span>
- [ ] <span style='color:#99cc66;background:背景颜色;font-size:文字大小;'>125.Valid Palindrome</span>

### 滑动窗口

- [ ] <span style='color:#9966ff;background:背景颜色;font-size:文字大小;'>3.Longest Substring Without Repeating Characters</span>
- [ ] <span style='color:#6699ff;background:背景颜色;font-size:文字大小;'>11.Container With Most Water</span>
- [ ] <span style='color:#6699ff;background:背景颜色;font-size:文字大小;'>76.Minimum Window Substring</span>
- [ ] <span style='color:#6699ff;background:背景颜色;font-size:文字大小;'>209.Minimum Size Subarray Sum</span>
- [ ] <span style='color:#6699ff;background:背景颜色;font-size:文字大小;'>239.Sliding Window Maximum</span>
- [ ] <span style='color:#6699ff;background:背景颜色;font-size:文字大小;'>713.Subarray Product Less Than K</span>
- [ ] <span style='color:#99cc66;background:背景颜色;font-size:文字大小;'>395.Longest Substring with At Least K Repeating Characters</span>
- [ ] <span style='color:#99cc66;background:背景颜色;font-size:文字大小;'>480.Sliding Window Median</span>
- [ ] <span style='color:#99cc66;background:背景颜色;font-size:文字大小;'>567.Permutation in String</span>
- [ ] <span style='color:#99cc66;background:背景颜色;font-size:文字大小;'>727.Minimum Window Subsequence</span>
- [ ] <span style='color:#99cc66;background:背景颜色;font-size:文字大小;'>Lint-604.Window Sum</span>

### 流处理

- [ ] <span style='color:#6699ff;background:背景颜色;font-size:文字大小;'>295.Find Median from Data Stream</span>
- [ ] <span style='color:#99cc66;background:背景颜色;font-size:文字大小;'>346.Moving Average from Data Stream</span>
- [ ] <span style='color:#99cc66;background:背景颜色;font-size:文字大小;'>352.Data Stream as Disjoint Intervals</span>
- [ ] <span style='color:#99cc66;background:背景颜色;font-size:文字大小;'>703.K-th Largest Element in a Stream</span>

### PreSum 前项和

- [ ] <span style='color:#9966ff;background:背景颜色;font-size:文字大小;'>53.Maximum Subarray</span>
- [ ] <span style='color:#6699ff;background:背景颜色;font-size:文字大小;'>238.Product of Array Except Self</span>
- [ ] <span style='color:#6699ff;background:背景颜色;font-size:文字大小;'>303.Range Sum Query-Immutable</span>
- [ ] <span style='color:#6699ff;background:背景颜色;font-size:文字大小;'>325.Maximum Size Subarray Sum Equal sk</span>
- [ ] <span style='color:#6699ff;background:背景颜色;font-size:文字大小;'>528.Random Pick with Weight</span>
- [ ] <span style='color:#6699ff;background:背景颜色;font-size:文字大小;'>560.Subarray Sum Equals K</span>

### 和差问题

- [ ] <span style='color:#9966ff;background:背景颜色;font-size:文字大小;'>1.TwoSum</span>
- [ ] <span style='color:#6699ff;background:背景颜色;font-size:文字大小;'>15.3Sum</span>
- [ ] <span style='color:#6699ff;background:背景颜色;font-size:文字大小;'>18.4Sum</span>
- [ ] <span style='color:#6699ff;background:背景颜色;font-size:文字大小;'>Lint-382.Triangle Count</span>
- [ ] <span style='color:#99cc66;background:背景颜色;font-size:文字大小;'>167.Two Sum II-Input array is sorted</span>
- [ ] <span style='color:#99cc66;background:背景颜色;font-size:文字大小;'>170.Two Sum III-Data structure design</span>
- [ ] <span style='color:#99cc66;background:背景颜色;font-size:文字大小;'>653.Two Sum IV-Input is a BST</span>
- [ ] <span style='color:#99cc66;background:背景颜色;font-size:文字大小;'>1099.Two Sum Less Than K</span>
- [ ] <span style='color:#99cc66;background:背景颜色;font-size:文字大小;'>259.3Sum Smaller</span>
- [ ] <span style='color:#99cc66;background:背景颜色;font-size:文字大小;'>Lint-573.Sum Closest</span>
- [ ] <span style='color:#99cc66;background:背景颜色;font-size:文字大小;'>Lint-443.Two Sum - Greater than target</span>
- [ ] <span style='color:#99cc66;background:背景颜色;font-size:文字大小;'>Lint-533.Two Sum - Closet to target</span>
- [ ] <span style='color:#99cc66;background:背景颜色;font-size:文字大小;'>Lint-587.Two Sum - Unique pairs</span>
- [ ] <span style='color:#99cc66;background:背景颜色;font-size:文字大小;'>Lint-609.Two Sum - Less than or equals to target</span>
- [ ] <span style='color:#99cc66;background:背景颜色;font-size:文字大小;'>Lint-610.Two Sum - Difference equals to target</span>







