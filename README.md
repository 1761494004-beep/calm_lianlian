# calm_lianlian

Calm Link MVP 本地演示版（按 `mvp.md` 实现）。

## 已实现（MVP 对齐）

- 连连看核心规则（最多 2 次转弯）
- 6 关递进挑战（4×6 → 8×10），每关独立时间与得分参数
- 轻松难度、提示、洗牌、无解自动洗牌
- 音效开关 + 环境音（雨声 / 白噪音）
- 游客试玩 1 局
- Google 登录（Demo Mock）
- Free 每日 5 局、Pro 无限局数（PayPal 订阅 Demo Mock）
- 结果弹窗 + 放松评分（1–5）
- 全站最短通关排行榜 Top 50（每用户仅保留最佳）
- MVP 埋点事件（记录在控制台与 localStorage）

## 运行

直接双击打开 `cartoon-lianliankan.html` 即可，或使用静态服务器：

```bash
python3 -m http.server 8000
# 打开 http://localhost:8000/project/calm_lianlian/cartoon-lianliankan.html
```

## 备注

当前为前端本地模拟版：登录、订阅、排行榜、埋点均存于 localStorage。
后续接入生产可替换为真实 Google OAuth、PayPal Subscriptions 与后端存储。
