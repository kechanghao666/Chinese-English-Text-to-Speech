# 中英文文本语音合成软件

Windows原生桌面程序，使用C++17和系统组件实现。

## 功能

- 输入和读取中英文文本
- 枚举并选择本机桌面发音人
- 按语言片段选择匹配语音
- 调节语速与音量
- 异步朗读、暂停、继续及停止
- 导出PCM WAV语音文件

## 编译与运行

准备Windows x64和MinGW-w64 C++工具链，在项目目录执行：

```powershell
.\build.ps1 -Compiler "C:\mingw64\bin\g++.exe"
.\SpeechReader.exe
```

也可将g++加入PATH后运行 `.\build.ps1`。工程另提供CMake配置。

## 操作

输入中英文文本或打开TXT，选择发音人，调节语速和音量。支持朗读、暂停、继续、停止及导出22050Hz、16位、单声道PCM WAV。自动中英文模式需要安装两种语言的桌面SAPI发音人。

## 文件

- src：窗口、处理算法及文件输入输出。
- build.ps1：Windows编译入口。
- CMakeLists.txt：CMake构建配置。

作者：柯长浩。仓库保留课程实验窗口标题。
