##Python版本切换（MAC）
* `python --version`显示当前运行的Python版本
* `which python`显示当前运行的python的directory path和版本
* `export PATH=/usr/bin:$PATH` 将python的路径切换为mac默认的
* 我的本机创建了一下aliases方便版本切换
 - `alias python2="export PATH=/usr/bin:$PATH"` 输入python2即切换到python2的路径，再输入python即可启动python
 - `alias python3="export PATH=/Users/hahah/anaconda/bin:$PATH"`输入python3即切换到python3的路径，再输入python即可启动python
 - homebrew安装的python2.7的路径在` PATH="/usr/local/opt/python/libexec/bin:$PATH"`

* 创建永久的alias
 - from the command line, open to edit the file by running the following:`nano ~/.bash_profile`
 or use`open -e .bash_profile` to open and edit it in Textedit.
 - Add the following lines either at the bottom of the file or wherever you’d like:
  ```alias python2="export PATH=/usr/bin:$PATH"```
  ```alias python3="export PATH=/Users/hahah/anaconda/bin:$PATH"```
 - Save and close the file. Now if you restart Terminal, the alias will be available to you. You can also tell Terminal to reload the `~/.bash_profile` file using the `source` command:
```source ~/.bash_profile```

 
**参考**

* [stackoverflow](https://stackoverflow.com/questions/3614898/switch-between-version-of-python)
* [Terminal/Bash Command-Line Shortcuts with Aliases](https://jonsuh.com/blog/bash-command-line-shortcuts/)
* [stackoverflow-How do I create a Bash alias?
](https://stackoverflow.com/questions/8967843/how-do-i-create-a-bash-alias)