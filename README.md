# gitools
git tools


## upfilelist.py

### 获取帮助

```
upfilelist --help
```

### 使用方式
> for svn

```
upfilelist author_name
upfilelist author_name num
upfilelist author_name since_num:
upfilelist author_name since_num:until_num
upfilelist clean

例：
upfilelist name             列出最近 50 个版本中用户 name 的修改记录
upfilelist name 100         列出最近 100 个版本中用户 name 的修改记录
upfilelist name 6230:       列出从版本号 6230 到最新版本之间用户 name 的修改记录
upfilelist name 6230:6280   列出从版本号 6230 到 6280 之间用户 name 的修改记录

upfilelist clean            将工作区所有的修改恢复初始状态
```

> for git

```
upfilelist author_name [since_time [until_time]]
upfilelist clean

例：
upfilelist name 10                    列出最近 10 个修改记录
upfilelist name 2018-03-01            列出 2018-03-01 之后的所有修改记录
upfilelist name 2018-03-01 2018-03-22 列出 0301 至 0325 之间的所有修改记录

upfilelist clean            将工作区所有的修改恢复初始状态
```
