# FIIO-DISC

FIIO DISC 社区固件与刷机资源。

## 当前版本：V439 Stable

V439 以 V427 Stable 为基线，主要修复：

- 蓝牙接收模式切歌后概率性断联、无法回连的问题；
- V32 遗留的两处 MIPS 延迟槽覆盖；
- 封面恢复分支每次命中造成的 32 字节栈泄漏；
- 息屏期间封面仍在后台旋转的问题。

息屏切歌后，亮屏时仍保留一次新封面刷新；没有新增蓝牙定时器。

固件、刷机工具和 SHA-256 校验值请从仓库的
[Releases](https://github.com/wanan522z/FIIO-DISC-/releases) 页面下载。

## R5 刷机工具说明

`FIIO-DISC-V427-Stable-OneClick-R5.zip` 是保持原样的 V427 R5 工具包。
需要刷入 V439 时，请在工具界面选择单独下载的
`FIIO-DISC-V439-Stable-rootfs.squashfs`；工具会根据所选固件自动生成 cfg。

刷机前建议备份原始 rootfs，并核对下载文件的 SHA-256。刷机存在风险，操作期间
不要提前断开 USB 或电源。
