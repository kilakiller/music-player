# 每日一曲 · 音乐分享播放器

为"每日音乐分享"视频录屏设计的网页播放器：左侧封面卡（封面 + 抽出的黑胶 + 进度控制），右侧歌词随播放滚动高亮。打开即用，无需安装任何东西。

## 直达链接

| 版本 | 链接 |
|------|------|
| **主版本 V6（两栏：封面卡 + 歌词）** | https://kilakiller.github.io/music-player/index-v6.html |
| V6 演示模式（自动加载示例歌曲） | https://kilakiller.github.io/music-player/index-v6.html?demo=1 |
| V5（横屏口播字幕版） | https://kilakiller.github.io/music-player/index-v5.html |
| V4（竖屏 9:16 抖音封面风） | https://kilakiller.github.io/music-player/index-v4.html |
| V3（唱片内页编辑风） | https://kilakiller.github.io/music-player/index-v3.html |
| V2（氛围光晕 + 环形频谱） | https://kilakiller.github.io/music-player/index-v2.html |
| V1（首版杂志风） | https://kilakiller.github.io/music-player/index-v1.html |

根地址 https://kilakiller.github.io/music-player/ 会自动跳转到 V6。

## 使用方法（V6）

1. 打开 V6 链接，点「选择音乐文件夹」，或直接把文件夹拖进窗口。
2. 文件夹里按**同名配对**放文件即可自动识别：

```
我的歌.mp3   ← 音频（mp3 / m4a / ogg / wav / flac）
我的歌.jpg   ← 封面（jpg / png / webp，可选）
我的歌.lrc   ← 歌词（可选，标准 LRC 时间轴格式）
```

- 没有同名图片 → 自动读取 mp3 内嵌的专辑封面
- 没有 .lrc → 自动读取 mp3 内嵌歌词（USLT，纯文本不滚动）
- 文件夹里放一张 `cover.jpg` → 所有歌共用这张封面

## 快捷键

| 键 | 功能 |
|----|------|
| `空格` | 播放 / 暂停 |
| `←` / `→` | 上一首 / 下一首 |
| `L` | 曲目列表（多首歌时） |

## 本地运行

直接双击 `index-v6.html` 也能用（选文件夹功能不受影响）；只有 `?demo=1` 演示模式需要通过 http 访问。

## 目录说明

- `index-v6.html` —— 当前主版本
- `music/` —— 示例歌曲（01 街灯唱片店 / 02 雨夜书桌，含封面与 LRC）
- `covers/`、`audio/` —— 各版本用到的封面与音频素材
- `使用说明.txt` —— 文件命名规则速查
