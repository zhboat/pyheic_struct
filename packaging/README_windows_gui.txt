LiveMotionPhotoManager Windows 版
================================

这是一个图形界面工具，用于批量处理 Live Photo / Motion Photo 媒体目录。

使用方式
--------
1. 解压 `LiveMotionPhotoManager-windows.zip`。
2. 进入解压后的 `LiveMotionPhotoManager` 文件夹。
3. 双击 `LiveMotionPhotoManager.exe`。
4. 在界面中选择要处理的照片目录。
5. 勾选需要执行的任务，然后点击“开始处理”。

ExifTool
--------
部分功能需要系统可以找到 `exiftool`，尤其是写入 MOV 的 ContentIdentifier、检测视频元数据、清理带 MotionPhoto_Data 标记的 MP4。

如果界面日志显示 exiftool 不可用，可以：

- 安装 ExifTool for Windows。
- 将 `exiftool.exe` 所在目录加入系统 PATH。
- 重新打开本程序。

注意事项
--------
- 首次运行时 Windows Defender SmartScreen 可能提示风险，确认来源可信后选择“仍要运行”。
- 建议先用少量照片测试，确认输出符合预期后再批量处理完整相册。
- 程序会根据所选任务生成转换文件、移动孤立视频或归档原始文件，请在处理前备份重要照片。
