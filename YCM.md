# YCM Install(Windows7)

### 1. Vim 8.1版本，并且支持Python3(+python3/dyn)
[Vim 8.1](https://github.com/vim/vim-win32-installer/releases) 
### 2. 安装python3(version3.7.4)
[Python](www.python.org) 
### 3. Vim和Python都使用64位
### 4. 通过Vundle安装YCM

遇到的一些问题及解决方案：

1. git clone 报错：error: RPC failed; curl 18 transfer closed with outstanding read data remaining 
    - git config --global http.postBuffer 524288000
2. Failed to recurse into submodule path 'third_party/ycmd'
    - [YCM ISSUE#1797](https://github.com/ycm-core/YouCompleteMe/issues/1797) 
    - 或者手动下载submodules，然后解压到相关文件夹
### 5. 安装CMake
安装CMake并添加到环境变量中

### 6. Visual Studio Build Tools 2019. During setup, select Visual C++ build tools in Workloads.
[Visual Studio 2019](https://visualstudio.microsoft.com/zh-hans/vs/) 注意，默认安装到c盘就可以

### 7. 编译
切换到YouCompleteMe根目录，执行下面命令
```shell
python install.py --clang-completer --java-completer
```

### 参考
[YCM README](https://github.com/ycm-core/YouCompleteMe#windows) 
