##文件操作
* `mkdir` -创建目录
* `rm` -删除
* rm 是Linux的删除命令
-r 指的是 递归删除
-f 指的是 强制删除
/* 指的是 根目录“/”下的所有文件
* `rm -rf file` -删除非空目录
* `mv` -移动
* `cp` -复制
* `cp -r` -复制目录
* `cd` -找到文件/目录位置
* `ls` -显示当前目录下的文件
* `find` -搜寻文件或目录
* `head -n 3 data.csv` -查看文件前面内容
* `tail -n 3 data.csv` -查看文件后面内容
* 使用`grep`查询文件内容
 - `grep 'data' todo.txt`
* `wc -l file` -统计行数
* `wc -w file` -统计单词数
* `wc -c file` -统计字符数
* 统计/home/han目录（包含子目录）下的所有js文件
 - `ls -IR /home/han |grep js| wc -|`
* `sort`排序
 - `-n` 按数字进行排序 VS `-d`按字典序进行排序
 - `-r` 逆序排序
 - `-k N` 指定按第N列排序
 - `sort -nrk 1 data.txt`
 - `sort unsort.txt | uniq` -消除重复行
* `cat text | tr '\t' ' '` -制表符转空格
* `cut -f 2,4 filename` -截取文件的第2，4列
* `paste file1 file2 -d` -按列拼接两个文件
* 改变文件编码
 - `iconv -f GBK -t UTF-8 file1 -o file2`