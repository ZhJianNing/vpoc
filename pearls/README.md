![pearls](pearls.jpg)

# 第一章 开篇
## 分析需求
### 怎样给一个磁盘文件排序？

* 直接用系统命令排一下呗？

不能使用系统命令

* 文件的内容是什么？

一个包含n个正整数的文件，
每个数都是7位 
大约有 10,000,000, 
这些数字不重复

* 能在内存里面排序吗？
内存只有1MB

10M * 4B = 40 MB




```bash
sort phone_numbers.txt
sort -g phone_numbers.txt
```




## 准确的问题描述
* 输入：一个包含n个正整数的文件，每个数都<n, n=10,000,000, 这些数字不重复
* 输出：按升序排列的输入的整数的文件，发现重复就报错
* 约束：内存大约1MB可用，磁盘空间充足，运行时间最多几分钟，最好可以在10秒内完成。
