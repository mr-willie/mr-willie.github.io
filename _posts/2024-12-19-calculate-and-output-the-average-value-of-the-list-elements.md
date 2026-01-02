---
layout: post
title: 计算并输出列表元素的平均值
tags: 
 - python
math: true
date: 2024-12-19 15:00 +0800
---

（简答题）从键盘输入一个列表，计算并输出列表元素的平均值。                            
这是某个学校的期末考试的题目。                          

### 解题思路分析：              

用``input()``让用户输入一串字符，然后用``split()``识别字符串的空格，把它们转化成列表。因为``split()``返回内容的是字符串列表，不是数值，所以我们需要用``float()``把字符串转化成可计算的数字。然后用``sum()``求和，用``len()``求平均值，最后``print()``输出。                  

### 答案                

```             
yonghushuru = input("输入列表数字，每个元素用空格隔开: ")

#把字符串转化成可计算的数字
liebiao = [float(num) for num in yonghushuru.split()]

zonghe = sum(liebiao)

average = zonghe / len(liebiao)

print(f"平均值为: {average}")
```             
