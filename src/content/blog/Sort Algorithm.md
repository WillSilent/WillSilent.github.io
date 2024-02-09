---
title: 'Sort Algorithm'
description: 'Summary of common sorting algorithms.'
pubDate: 'Feb 08 2024'
heroImage: '/post_img.webp'
tags: ['algorithm', 'sort']
---

# Common Sort Algorithm

### Bubble Algorithm

![Animation](/img/bubbleSort.gif 'Bubble Sort')

```
function bubbleSort(arr) {
   var len = arr.length;
   for (var i = 0; i < len - 1; i++) {
       for (var j = 0; j < len - 1 - i; j++) {
           if (arr[j] > arr[j+1]) {        // 相邻元素两两对比
               var temp = arr[j+1];        // 元素交换
               arr[j+1] = arr[j];
               arr[j] = temp;
           }
       }
   }
   return arr;
}
```
