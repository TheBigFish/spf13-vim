# spf13-vim

thebigfish's fork from Steve Francia's Vim Distribution [README](https://github.com/spf13/spf13-vim/blob/3.0/README.markdown)

## install for windows

### python

python3.5.4 64bit  
对应网盘文件 *python-3.5.4-amd64.exe*  
python 要起一个ycm后台  

### gvim

gvim 版本需要大于 8.0， 并且支持python2、python3  
下载编译好的版本：

[Windows Vim binaries](https://tuxproject.de/projects/vim/)
对应网盘文件 *complete-x64-vim8.1.exe*  
解压至任意文件夹  
检测配置环境变量是否支持python  

```bash
:py3 print('hello')
hello
:py print('hello')
hello
```

### ycm

下载已经编译好的版本  
[YouCompleteMe-for-windows](https://github.com/CuriousFu/YouCompleteMe-for-windows.git)  
对应网盘文件 *YouCompleteMe-python3.5.7z*  
解压至 bundle 文件夹 如`C:\Users\bigfish\.vim\bundle`  
spf13 中已经配置好 youcompleteme 选项  

### 安装 spf13

- 下载 [spf13-vim-windows-install.cmd](https://github.com/TheBigFish/spf13-vim/blob/3.0/spf13-vim-windows-install.cmd)
- 管理员模式打开 cmd 然后运行安装
- 会同时安装 youcompleteme 插件。插件安装后手动删除此插件
- 将 YouCompleteMe-for-windows 对应的文件解压至安装 bundle 文件夹

## 安装 msys1.0

对应网盘文件 *MSYS-1.0.10*
加入path

### 不确定是否是必须的步骤

已安装 LLVM-9.0.0-win64.exe
已安装 Microsoft Visual C++ Redistributable 2017 （VC_redist.x64.exe）

## 快捷键

<ctrl+e> NERDTreeTabsToggle

- ycm:
  - `<leader>l` : 跳转到声明
  - `<leader>f` : 跳转到定义
  - `<leader>g` : 跳转到定义或声明

- cscope
  - `<leader>fa`: 交互式查找
  - `<leader>l` : 局部列表
  - `<leader>fs`: Find this C symbol
  - `<leader>fg`: Find this definition
  - `<leader>fd`: Find functions called by this function
  - `<leader>fc`: Find functions calling this function
  - `<leader>ft`: Find this text string
  - `<leader>fe`: Find this egrep pattern
  - `<leader>ff`: Find this file
  - `<leader>fi`: Find files #including this file