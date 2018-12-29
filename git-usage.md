#### **配置 \(~/.gitconfig\)**

\[core\]

```
editor = vim
```

/\* 免密push - 需在~/.git-credentials里设置[https://用户名:密码@github.com](https://用户名:密码@github.com)  
 \*/

\[credential\]

```
helper = store
```

/\* 设置git commit时自动打开的模板 \*/

\[commit\]

```
   template = ~/.gitmessage
```

#### Tip

##### git log:

**图形化显示**

git log --graph

**显示对应代码改动**

git log -p

##### git tag:

**显示tag和commit id的对应关系**

git show-ref --tags

**根据tag查询commit id**

git show &lt;tag&gt;

**根据修改生成patch**

git format-patch \(比如HEAD^\)

