# 永恒玫瑰 · Eternal Rose

粒子渲染的玫瑰花束——花店风格的螺旋穹顶花束，用纯 Web 技术构建。

## 效果

- **9 朵玫瑰** 螺旋穹顶构图：正红冠花全开 → 珊瑚/艳粉/蜜桃环带 → 酒红半开 → 双花蕾
- **花店元素**：奶白纸锥包装、深红缎带蝴蝶结、满天星、晨露碎钻
- **绽放动画**：12.7 秒从花苞到全开，内层先开、外层后开
- **氛围**：香槟波凯背景光斑、景深虚化、飘落花瓣

## 技术

- **双引擎渲染**：WebGL 优先（GPU 粒子 + 景深），Canvas2D 自动降级
- **~152K 粒子**（WebGL）/ ~35K（Canvas2D）
- 纯静态 HTML + CSS + JS，无构建、无依赖

## 运行

直接用浏览器打开 `eternal-rose.html` 即可。

或本地起服务：

```bash
python3 -m http.server 8000
# 打开 http://localhost:8000/eternal-rose.html
```

## 操作

- **点击画面** → 重新绽放
- **R** → 重新绽放
- **REC** → 录制（WebGL 模式下输出 WebM）

## 文件

```
eternal-rose.html   单文件全实现（粒子系统 + 双引擎 + HUD）
```

## License

MIT
