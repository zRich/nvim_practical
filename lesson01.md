# Content

## File

存放在硬盘上的文件。

## Buffer

文件打开后载入Buffer，编辑的是Buffer，通过write写入文件。

| 命令    | 缩写命令    | 功能    |
|---------------- | --------------- | --------------- |
| ls     | -    | 查看所有Buffer    |
| bfirst    | bf     | 加载第一个Buffer到当前窗口    |
| blast |   bl  | 加载最后一个Buffer |
| bnext   | bn    | 加载下一个Buffer   |
| bprevious   | bprevious    | 加载下一个Buffer   |
| bdelete | bd | 删除当前Buffer |
| new | n | 新建Buffer |
| quit | q | 退出Buffer |
| write | w | 将Buffer写入文件 |

## Window
- <C-W> 前导建
- <C-W> + 

| 命令    | 命令缩写    | 功能    |
|---------------- | --------------- | --------------- |
| <C-W> + s     |     | 左右拆分窗口    |
| <C-W> + v    |     | 


## Mode
- Normal: 普通模式，也是默认模式
- Insert：插入模式，buffer处于编辑状态
- Command： 命令模式，接受用户输入的命令

返回Normal模式：ESC键
进入Command模式：**：** 键
进入Insert模式：i 在当前位置插入，A在行尾插入

## Commands

| 命令    | 命令缩写    | 功能    |
|---------------- | --------------- | --------------- |
| h     |      | 左移    |
| l     |      | 右移    |
| k   |      | 上移   |
| j   |      | 下移   |


# Command Patterns

将模式，命令等组合

{part1}{part2}{part3}{...}
例如

 __:vnew__

其中：
- **:** 表示命令模式，后面输入的是命令
- v 表示vertical，左右拆分
组合的结果是新建一个buffer，并左右拆分窗口

__<C-W> + v__

左右拆分窗口
