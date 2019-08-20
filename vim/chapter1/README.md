# Getting started

## Basics

```
$ git vimtutor
```

进入vim tutorial

### 1.1 Moving

| 方向键          | vim  |
| --------------- | ---- |
| $$\uparrow$$    | k    |
| $$\downarrow$$  | j    |
| $$\rightarrow$$ | l    |
| $$\leftarrow$$  | h    |

如果能使用方向键，尽量使用方向键

### 1.2 Exiting

1. `esc`回到normal mode
2. `:q!`，`Enter`不保存并退出

### 1.3 Text Editing

#### Deletion

1. 将光标移动到要删除的character上
2. `x`删除该character

#### Insert

1. 将光标移动到要插入character位置之后
2. `i`进入插入模式
3. 完成后`esc`

#### Append

与Insert类似，只不过用`a`

### 1.4 Editing a file

1. 新建file使用`vim <filename>`
2. 编辑文件
3. `:wq`保存并退出

## 2 Commands

### 2.1 Delete a word

1. 按`esc`确保在noraml mode
2. 将光标移动到word的开始
3. 按`dw`删除单词

### 2.2 Delete a sentence

1. 将光标移动到句子的开始
2. 按`d$`

### 2.3 On operators and motions

1. `d`是opeator
2. `w`是motion

### 2.4 Use a count for a motion

- `2w`表示将光标向前移动2个word的头部
- `3e`表示将光标向前移动3个word的尾部
- `0`表示移动到某句的开始

### 2.5 Use a count to delete mode

- 基本模式：d   number   motion

### 2.6 Operating on lines

- `dd`删除一行
- number dd：删除多行

### 2.7 The undo commands

- `u`修复一次command
- `U`修复整行
- `ctrl+y`：`ctrl+r`



