# UICS2021

这是 UICS2021 的 C++17 CMake 工程。当前运行目标 `UICS2021` 是用于验证构建环境的占位程序，运行后输出 `Hello, World!`。

## 在另一台主机用 CLion 打开

1. 在 CLion 启动页选择 **Get from VCS** 或 **Clone Repository**，输入下列地址。也可以在终端运行：

   ```sh
   git clone https://github.com/zhuchenyang666/UISC2021.git
   cd UISC2021
   ```

2. 在 CLion 里打开克隆后的根目录，目录内应有 `CMakeLists.txt`。
3. 如果 IDE 提示配置工具链，在 **Settings → Build, Execution, Deployment → Toolchains** 中选择此主机的 x64 C++ 工具链。Windows 上可使用 CLion 的 MinGW 工具链，或已安装 C++ 工作负载与 Windows SDK 的 MSVC 工具链。使用 CLion 自带的 CMake，或本机 CMake 3.16 及以上版本。
4. 在 **CMake** 设置里为 Debug 配置选择该工具链。加载完成后，在运行配置中选择 `UICS2021`，点击 **Run**。

## 使用命令行构建

将支持 C++17 的编译器和 CMake 加入当前构建环境。使用 MSVC 时可在 x64 开发者命令提示符中运行：

```sh
cmake -S . -B build
cmake --build build --config Debug
```

本机的 CLion 设置和 CMake 构建目录由各自的环境生成。
