## 快速启动

启动命令及参数

```sh
java -jar Scanner.jar -r <rpodir> 
```

repodir: 待扫描的项目文件目录路径（包含.git子文件夹，即可使用git checkout切换版本）



输出：

1. commit-msg.csv：该目录下所有commit的提交标题。
2. fix-commit.csv：根据提交信息得出的可能是缺陷修复的commit id。
3. test-commit.csv：存在测试用例修改或添加的commit id。
4. intersection-commits.csv：2和3的交集。

运行时间参考：7000commits的项目大致15秒。
