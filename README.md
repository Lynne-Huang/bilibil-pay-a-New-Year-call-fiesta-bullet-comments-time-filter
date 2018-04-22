# 2015bilibili拜年祭弹幕时间分析

数据由[QTNiCheng](https://github.com/QTNiCheng/bilibili_danmu "项目地址")  <br/>
用python爬虫获得的数据。数据仅节选时间部分，并未对内容进行分析

 ## 程序思路
 1. 分组->统计->排序<br>
 2. 将文件传入，因为要知道具体数据是什么此处选用字符流，字符流 java中字符编码是Unicode，可以识别奇怪的字符<br>
 3. 用字符流注意配合使用缓冲区<br>
 4. 将所有数据传入ArrayList(其实就是一个动态数组<br>
 5. 利用Map不可重复key的特点，键值来存储重复的次数<br>
 6. 对map排序treemap<br>
 7. 键值升序排序输出<br>
 
## 程序运行结果分析

![程序运行结果](https://github.com/Lynne-Huang/bilibil-pay-a-New-Year-call-fiesta-bullet-comments-time-filter/blob/master/哔哩哔哩弹幕测试运行结果.png "运行结果")
### 由图可知：
 1. 在头10分钟里总共发了1048576条弹幕（数据量还是很可怕的<br>
 2. 在9：54秒开始，弹幕数突然由千条弹幕上升到万条甚至2万条弹幕，可见此时应该是第一个节目的开始，或者是集体喊出口号：哔哩哔哩 (゜-゜)つロ 干杯~-bilibili<br>
 3.在9分57秒的时候弹幕数量是前10分钟之最 21358<br>
 4.整个程序运行0.462s  这个方法来统计数据还是很快的，第一次写的时候用，读一条匹配加一的方法，快好几倍，具体数据忘了<br>
 5.这个程序是[QTNiCheng](https://github.com/QTNiCheng "GitHub地址") 在线上问我Java能否实现python中一个排序小工具，然后自己写了一个<br>
[程序运行结果]:https://github.com/Lynne-Huang/bilibil-pay-a-New-Year-call-fiesta-bullet-comments-time-filter/blob/master/%E5%93%94%E5%93%A9%E5%93%94%E5%93%A9%E5%BC%B9%E5%B9%95%E6%B5%8B%E8%AF%95%E8%BF%90%E8%A1%8C%E7%BB%93%E6%9E%9C.png
