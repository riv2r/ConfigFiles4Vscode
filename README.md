# 用于vscode的C++程序开发的配置文件设置

## 编译环境准备

首先要在本机下载安装C++编译环境：

> Visual Studio 的 MSVC
>
> mingw-w64

对于直接安装`Visual Studio`中`C++`程序开发模块的情况来说，虽然会携带安装`MSVC`，但是使用`MSVC`作为`vscode`的`C++`编译环境，不是很方便，需要首先打开`Developer Command Prompt`，在从这里面使用`code`命令打开`vscode`，才能正常使用`MSVC`

所以，采用`mingw-w64`是比较方便的，只需要在最一开始将其配置好就可以

> emmm我这里其实mingw和mingw-w64都是下载过的，但是mingw感觉明显老态龙钟，安装比较麻烦，也不支持64位程序，还是mingw-w64比较好

## 配置文件编写

### c_cpp_properties.json

打开`vscode`，按下`ctrl+shift+p`打开，在输入框中输入`C/C++`，在下拉菜单中可以看到`Edit Configurations(UI)`，点击进入

PS 可以不用图形界面，但是其实挺方便的

- 在编译器路径下拉菜单中，找到`g++`
- `IntelliSense`模式，选择`gcc-x64`

配置完成

### tasks.json

打开`vscode`，按下`ctrl+shift+p`打开，在输入框中输入`tasks`，在下拉菜单中可以看到`Configure Default Build Task`，点击，选择其中的`g++`选项，配置完成

### launch.json

打开`vscode`，按下`F5`，自动生成调试所用的配置文件

