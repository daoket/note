# 灵犀 JSSDK 常见问题

1. IOS 版灵犀 base64 播放问题

```
lx.playVoice({
  resId: 'url', // IOS 版不支持 base64 格式
  type:'1'
});
```

建议使用 video 标签替代，手动点击

2. IOS 版灵犀音频和视频无法同时播放
复现：原生 video 播放视频时，调用 lx.playVoice 播放背景音，视频会停止
解决方案：1. 联系客户端修复 2. 播放视频时，禁止背景音播放
