# 可复用结果

## 当前快照仓库

- GitHub：
  - `https://github.com/uplinkira/micro-mirror-deploy.git`
- 定位：
  - `2026-03-14` 深圳黑客松快照
  - 发布镜像与历史档案

## 长期主仓库

- 计划 GitHub：
  - `https://github.com/uplinkira/vitalscope.git`
- 定位：
  - 长期单人产品仓库
  - source of truth
- 维护者：
  - `uplinkira`

## 快照团队信息

- `uplinkira`
- `2` collaborating bioinformatics graduate researchers from the Chinese Academy of Sciences

## 快照比赛信息

- 时间：
  - `March 14, 2026`
- 地点：
  - `Shenzhen, China`
- 结果：
  - according to team records, `General Track First Place`

## 推荐仓库结构

- 以后只在 `vitalscope` 继续开发
- `micro-mirror-deploy` 只保存比赛快照、部署镜像和历史说明

## 稳定命令

- 运行当前快照站点
  - `cd D+20260314+goat/micro-mirror-deploy && python3 -m http.server 8000`
- 运行未来主仓库站点
  - `cd D+20260314+goat/vitalscope && python3 -m http.server 8000`
