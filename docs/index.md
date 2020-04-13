# 算法导论第三版  
## 一些问题
当本地仓库和远程仓库不同步时，`mkdocs gh-deploy`时，会报错
```py
UnicodeDecodeError: 'utf-8' codec can't decode byte 0xb7 in position 44: invalid start byte
```
这并无大碍，依旧可以生成网页，该网页与本地仓库的代码保持一致。如果其他时间在网页上编辑过某些md文件，可pull到本地后再在本地`mkdocs gh-deploy`。相比于readthedocs，mkdocs相对繁琐，但免费用户没有广告。
## 致敬  
非常感谢此项目fork自：https://github.com/walkccc/CLRS 。 在此用于自己学习《算法导论》。  
## 如何生成本站  
依 [walkccc](https://github.com/walkccc/CLRS) 所言，参照 [MkDocs](http://www.mkdocs.org/)  ，经过一番折腾后步骤如下：  
1. `pip install -i https://pypi.tuna.tsinghua.edu.cn/simple mkdocs`  
2. 远程新建本仓库
3. `git clone https://github.com/walkccc/CLRS` 
4. 删除本地CLRS中的.git文件夹，`git init`, `git remote add origin https://github.com/cjql/algorithm`    
5. 用vsc打开整个文件夹CLRS，将所有`walkccc`替换为自己的用户名，将所有的`CLRS`替换为本仓库的仓库名   
6. 将本地仓库同步到GitHub上的本仓库  
7. 在shell里面键入`mkdocs gh-deploy`  
8. 修改各个md文件，push ，`mkdocs gh-deploy`，循环往复。  
## 相关资源
the bible textbook - [**Introduction to Algorithms** _Third Edition_](https://mitpress.mit.edu/books/introduction-algorithms-third-edition), published by [Thomas H. Cormen](https://mitpress.mit.edu/contributors/thomas-h-cormen), [Charles E. Leiserson](https://mitpress.mit.edu/contributors/charles-e-leiserson), [Ronald L. Rivest](https://mitpress.mit.edu/contributors/ronald-l-rivest), and [Clifford Stein](https://mitpress.mit.edu/contributors/clifford-stein).  


## License  

Licensed under the MIT License.  