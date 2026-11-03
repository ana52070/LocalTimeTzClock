# v16 Build 26300 受控测试包

仅用于 PR #2 真机验收，尚非正式发布。构建源码对应本地提交 f023ab8f4f2e4dbf84f7812b254275096ac97cc1，20 项自动化测试与 MSVC 构建通过，不代表真机验收通过。

本测试分支基于主分支，仅存放测试附件，不代表该分支源码是 v16；不要在此分支直接构建根目录源码来测试 v16。

请下载本目录 ZIP，核对 SHA256SUMS.txt 后解压，并阅读包内《开始验证.md》。x64 SystemTray.dll 2609.11000.100.0 的 SHA-256 应为 9772d19ec44f22ab2fcb976941d6ba6d1e66aabfb9d66367723bb9154ce7769f。

先在旧版目录执行 tzclock.exe stopwatch 和 tzclock.exe off，再保存工作，通过任务管理器重启 Windows 资源管理器，卸载旧 DLL。不要同时运行旧版 watch；仅 off 不会卸载 DLL。随后从独立的新目录运行 v16。本次不运行 install/watch、不改系统时区。
