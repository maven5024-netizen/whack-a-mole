# 🔨 打地鼠 Whack-a-Mole

一个用纯 HTML + CSS + JavaScript 写的打地鼠小游戏,无需安装、无需构建,单文件即可运行。

🎮 **在线试玩**:[https://maven5024-netizen.github.io/whack-a-mole/](https://maven5024-netizen.github.io/whack-a-mole/)

<!-- 在这里放一张截图:![截图](screenshot.png) -->

## 玩法

- 限时 30 秒,点击(或触屏)冒出来的目标得分。
- 🐹 普通地鼠 **+10** 分
- 🌟 金鼠 **+30** 分
- 💣 炸弹 **-20** 分,并断掉连击
- 连续命中累积连击,每满 5 连击额外加分(最多 +10)
- 三档难度:简单 / 普通 / 困难
- 最高分保存在浏览器本地(`localStorage`)

## 运行

直接用浏览器打开 `index.html` 即可:

```bash
open index.html
```

或者启动一个本地服务器:

```bash
python3 -m http.server 8000
# 然后访问 http://localhost:8000
```

## 自定义

所有逻辑都在 `index.html` 中:

- `GAME_TIME`:游戏时长(秒)
- `LEVELS`:各难度的停留时间、间隔和同时出现的数量
- `pickType()`:地鼠 / 金鼠 / 炸弹的出现概率
- 想换成自己的图片,把 `.mole` 里的 emoji 替换成 `<img>` 即可

## 许可证

[MIT](LICENSE)
