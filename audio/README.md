# 音乐播放器使用说明

请将您的音频文件放入此目录，支持的格式包括：
- MP3
- WAV
- OGG
- M4A

## 示例文件
您可以将音频文件重命名为以下名称来快速开始：
- sample1.mp3
- sample2.mp3

或者修改 `assets/ts/main.ts` 文件中的 `sampleTracks` 数组来指定您自己的音频文件。

## 配置音乐列表
在 `assets/ts/main.ts` 的 `initMusicPlayer` 函数中，您可以修改音乐列表：

```typescript
const sampleTracks: Track[] = [
    {
        title: "您的音乐标题",
        artist: "艺术家名称", 
        src: "/audio/your-music-file.mp3"
    },
    // 添加更多音乐...
];
```

## 功能特点
- 跨页面持续播放
- 音乐播放状态会保存到本地存储
- 支持播放/暂停、上一首/下一首
- 支持音量控制和进度条
- 支持暗色/亮色主题
- 响应式设计，适配移动设备
