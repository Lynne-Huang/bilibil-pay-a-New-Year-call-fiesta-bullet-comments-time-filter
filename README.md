# 2015bilibili拜年祭弹幕时间分析

数据由[QTNiCheng](https://github.com/QTNiCheng/bilibili_danmu "项目地址")  <br/>
用python爬虫获得的数据。数据仅节选时间部分，并未对内容进行分析

 ## 程序思路
 * 分组->统计->排序<br>
 * 将文件传入，因为要知道具体数据是什么此处选用字符流，字符流 java中字符编码是Unicode，可以识别奇怪的字符<br>
 * 用字符流注意配合使用缓冲区<br>
 * 将所有数据传入ArrayList(其实就是一个动态数组<br>
 * 利用Map不可重复key的特点，键值来存储重复的次数<br>
 * 对map排序treemap<br>
 * 键值升序排序输出<br>
 
