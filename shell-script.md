## Shell

+ 设置变量
  + 只读：readonly
  + 删除：unset
+ 引用变量
  + 本身：$、${val}
  + 长度：${#val}
  + 变量替换：
    + ${val-default}：未定义 -> 返回default
    + ${val:-default}：未定义、为空 -> 返回default
    + ${val:=default}：未定义、为空 -> 修改val、返回default
    + ${val:+default}：已定义不为空 -> 返回default
    + ${val:?massage}：未定义、为空 -> 输出message到stdout
+ 字符串
  + 无引号：
  + 单引号：原样输出
  + 双引号：允许引用变量、转义
  + 拼接：直接拼接
  + 截取：${val:0:n}
+ 数组
  + 设置：arr=(val1 val2 val3)
  + 引用：${arr[0]}
  + 引用所有元素：${arr[*]}、${arr[@]}
  + 数组长度：#
+ 转义
  + \
  + ``：命令替换
+ 运算符
  + 不支持数字运算，使用内建命令完成
  + 条件表达式放在方括号内
  + 数关系运算符：-eq、-ne、-gt、-lt、-ge、-le
  + 布尔运算：-a、-o、！
  + 逻辑运算：&&、||
  + 字符串运算：=、!=、-z、-n、str
  + 文件测试运算：
    + b块设备、-c字符设备、-d目录、-f普通文件、-g是否设置sgid、
    + k是否设置sticky bit、-p是否为具体名管道、-u是否设置suid、
    + r是否可读、-w是否可写、-x是否可执行、-s是否为空、-e是否存在
+ 流程控制：
  + if condition then elif then else fi
  + for val in arr do done
  + while  condition do done
  + unti condition do done
  + true、false、break、continue、until
  + case val in pattern1) ;; pattern2) ;; *) ;; esac
+ 函数：
  + [ function ] funname [()] { action;[return ;]}
  + 函数名、参数：$0、$1、$2、…、${n}
  + 参数长度：$#
  + 参数字符串：$*、$@（使用时加引号）
  + 当前进程号：$$
  + Shell当前可选项：$-
  + 最后退出状态：$?


+ 内建命令
  + ehco -s：转义字符串
  + printf：c printf移植
  + expr：求值
  + include file：文件包含
