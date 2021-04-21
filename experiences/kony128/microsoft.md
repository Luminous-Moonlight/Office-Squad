# Akuna

## C+AI (Cloud And AI) 2021 Summer Internship

> Position: Software Development Intern (Dynamics 365)
> 
> Focusing: Developing Skills, Willingness To Work
> 
> Process: Three 45 minutes online interviews

## 一面

### 面试启动

1. 面试官自我介绍，面试官所在部门负责金钱相关，可能包括付款过程等等
2. 面试官要求面试以英文进行
3. 面试官要求面试者英文自我介绍

### 简历相关

1. 作为项目负责人，有没有遇到过团队问题，比如团队矛盾；是啥么解决的

### 基础知识相关

1. 简述一下 LSM 树和 B+ 树区别

### 算法题

````c++
/*
 * Input: Given two integer arrays, please exchange a pair of values (one value in each array) so that the sum of all elements of the two arrays is equal.
 * Array1 = [4, 1, 2, 1, 1, 2]
 * Array2 = [3, 6, 3, 3]
 * Output: Returns an array, the first element is the element to be swapped in the first array, and the second element is the element to be swapped in the second array.
 * [1, 3]
*/

// Shoud use Hash Map instead of red black tree to sort
// This version of code is lack of corner cases handling
vector<int> arrayAndSwap(vector<int> a1, vector<int> a2) {
  // sort a1 and a2
  bool swapped = false;
  vector<int> res;
  int sum1 = 0;
  int sum2 = 0;
  multiset<int> sort1, sort2;
  for (auto iter = a1.begin(); iter != a1.end(); iter++) {
    sort1.insert(*iter);
    sum1 += *iter;
  }
  for (auto iter = a2.begin();iter != a2.end(); iter++) {
    sort2.insert(*iter);
    sum2 += *iter;
  }
  // swap 1 and 2 to make sure 1 is less than 2
  if (sum1 > sum2) {
    int tmp = sum1;
    sum1 = sum2;
    sum2 = tmp;
    multiset<int> tmpSort = sort1;
    sort1 = sort2;
    sort2 = tmpSort;
    vector<int> tmpArr = a1;
    a1 = a2;
    a2 = tmpArr;
    swapped = true;
  }
  // calculate difference and find the result
  int diff = (sum2 - sum1) >> 1;
  for (auto iter = sort1.begin(); iter != sort1.end(); iter++) {
    // can't find in arr2, just skip
    if (sort2.find(*iter + diff) == sort2.end()) {
      continue;
    } else {
      if (!swapped) {
        res.push_back(*iter);
        res.push_back(*iter + diff);
      } else {
        res.push_back(*iter + diff);
        res.push_back(*iter);
      }
      break;
    }
  }
  return res;
}
````

### 复盘

1. 英文口语太烂，必须在项目上，自我介绍上，相关工作上做充足的准备
2. 面试前应该调试好面试物理环境和编程环境，不要有各种问题，不然双方都很不爽

## 二面

### 面试启动

1. 面试官自我介绍
2. 要求面试者英文介绍

### 简历相关

1. 介绍一下项目中遇到的难点

### 算法题

````c++
/* CPU scheduling
 * A single core CPU with single thread
 * A bunch of tasks with params of TI and PI:
 * eg. [[1, 2], [2, 3], [3, 4] ...] 
 * (arrive time and process time)
 * You need to output the executing indexes to acquire minimum total CPU execution time
 */
````

### 复盘

1. 必须将语言特性，比如 C++, Python, GoLang 的特性，包括排序，标准库，各种面向对象打包编程等等熟悉一下
2. 基础的数据结构还是得多熟悉一下，不能偷懒

## 三面

### 面试启动

1. 面试官自我介绍，面试官介绍部门
2. 面试官要求面试者英文介绍

### 沟通相关

1. 用英文介绍一下自己在学校最喜欢的课程

### 算法题

````c++
/* A random integer array need to be divide into two parts
 * The sum of left part is equal to the sum of right part
 * Find the index of the division 
 * (number at the index is not included by any parts)
 */
````

### 复盘

1. 面试官说我的英文实在是太烂了，一定要好好弄英文口语和听力