# 灵犀 JSSDK 常见问题

1. IOS版灵犀 base64 播放问题

```
lx.playVoice({
  resId: 'url', // IOS 版不支持 base64 格式
  type:'1'
});
```

建议使用 video 标签替代，手动点击

2. 
