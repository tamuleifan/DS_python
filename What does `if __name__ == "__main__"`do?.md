### What does `if __name__ == "__main__"`do?
python通过命名空间的方式实现module的高效运行。

由于一个模块或包可能会在一个程序中的不同位置多次引用，所以python第一次引入模块时对其进行缓存，而不是每次都执行模块中的代码，这样应用程序的模块化和良好的代码组织可以实现代码的高效运行。

总结：python第一次引入一个模块时，会run它并且缓存它，如果之后这个program was used，会run它，如果program was imported from another module，就不会run它，而是用缓存里的。

这个模块如果被调用后，又做了更改，就要reload（）或者dreload（），以更改缓存中的内容。（**利用python进行数据分析P77**）

参考资料

* [What does `if __name__ == "__main__"`do?](https://stackoverflow.com/questions/419163/what-does-if-name-main-do)
* [A module's `__name__`](http://ibiblio.org/g2swap/byteofpython/read/module-name.html)

