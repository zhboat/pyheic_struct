LiveMotionPhotoManager macOS 版
==============================

这是一个图形界面工具，用于批量处理 Live Photo / Motion Photo 媒体目录。

使用方式
--------
1. 解压 `LiveMotionPhotoManager-macos.zip`。
2. 打开解压后的 `LiveMotionPhotoManager-macos` 文件夹。
3. 双击 `LiveMotionPhotoManager.app`。
4. 在界面中选择要处理的照片目录。
5. 勾选需要执行的任务，然后点击“开始处理”。

首次运行
--------
从网络下载的 app 可能会被 macOS 标记为隔离。如果无法直接打开，可以在终端进入解压目录后执行：

```bash
xattr -dr com.apple.quarantine LiveMotionPhotoManager.app
```

ExifTool
--------
部分功能需要系统可以找到 `exiftool`，尤其是写入 MOV 的 ContentIdentifier、检测视频元数据、清理带 MotionPhoto_Data 标记的 MP4。

macOS 可通过 Homebrew 安装：

```bash
brew install exiftool
```

安装后重新打开本程序。

注意事项
--------
- 当前构建未做 Apple Developer ID 签名和公证，首次打开时可能需要在“系统设置 > 隐私与安全性”中允许。
- 建议先用少量照片测试，确认输出符合预期后再批量处理完整相册。
- 程序会根据所选任务生成转换文件、移动孤立视频或归档原始文件，请在处理前备份重要照片。
