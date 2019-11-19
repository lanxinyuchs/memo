!$ 上一个命令的最后一个参数
!:n 上一个命令的第n个参数
!* 上一个命令的所有参数

重复执行一条命令：
while true; do free -m; sleep 3; done

##### 规则

起始 \#！

以空格分隔字符串，否则使用引号

多个命令之间使用分号

单行注释\#

多行注释&gt;&gt;

##### 快捷键

ALT+B 光标向后移动一个单词

ALT+F 光标向前移动一个单词

CTRL+U 删除光标左边部分

CTRL+K 删除光标右边部分

CTRL+W 删除光标左边的单词

##### $符号

$0 命令本身（可用echo "$0"获取当前shell类型）

$@ $\* 所有参数

获取变量的值** **${varible}  变量名相当于指针

双引号展开，单引号不展开

**获取命令输出**

var=\`command\`

var=$\(command\)

**控制结构**

if \[ commnad  \]; then \(注意空格，可用test代替\)

elif ; then

else

fi

###### **Tips**

!\* 使用上一条命令的参数

ctrl+r 根据输入动态搜索历史命令

**快捷键**

alt+b 后退 alt+f 前进

##### 函数

func\(\) { xxx }

例如 cd\(\) { builtin cd "$@" && ls; }

**常用alias \(~/.bashrc\)**

```
alias rm="rm -f"
alias la="ls -a --color"
alias ll="ls -al --color"
alias mytree="tree -L"
alias mydu="du -h --max-depth=1"
alias fname="find . -name"
alias fgrep="find .|grep"
alias fxargsgrep="find .|xargs grep -r"
alias ..="cd .."
alias ...="cd ../.."
alias grep="grep -n --color"
```

**设置环境变量 \(~/.bashrc\)**

export USER\_ENV=""

###### **注意**：等号两边无空格

环境变量使用冒号分割

添加PATH  export PATH="$PATH: new"

#### 



