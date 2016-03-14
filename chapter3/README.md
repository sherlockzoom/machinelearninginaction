决策树（decision tree）是一个树结构（可以是二叉树或非二叉树）。其每个非叶节点表示一个特征属性上的测试，每个分支代表这个特征属性在某个值域上的输出，而每个叶节点存放一个类别。使用决策树进行决策的过程就是从根节点开始，测试待分类项中相应的特征属性，并按照其值选择输出分支，直到到达叶子节点，将叶子节点存放的类别作为决策结果。

> 决策树伪代码

```
测试数据集中的每个子项是否属于同一个分类：
	if so return 类标签：
	else
		寻找划分数据集最好的特征
		划分数据集
		创建分支节点
			for 每个划分的子集
				调用函数createBranch并增加返回结果到分支节点中
		return 分支节点
```