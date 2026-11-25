# Risk Zoo 介绍站

本仓库是 **Risk Zoo**（投资组合持仓管理与风险分析系统）的公开介绍页源站，仅承载产品说明、架构介绍与计算口径，不包含原项目的任何源码、配置、数据或 git 历史。

在线地址：[https://bnycx.github.io/risk-zoo/](https://bnycx.github.io/risk-zoo/)

## 内容边界

- 页面中的图表均为原创示意图，不含真实持仓、真实收益或账户信息。
- 不复制原项目的源码文件、环境变量、缓存文件、数据库或测试夹具。
- 对外口径固定为「5 类正式优化器 / 7 个 Draft run entries」；有效前沿属于可视化，不是独立优化器。
- 第三方组件只在功能层面描述，不分发其源码；声明见 [NOTICE.md](NOTICE.md)。

## 本地预览

本页为纯静态 HTML/CSS，无构建步骤、无外部 CDN 依赖：

```bash
python3 -m http.server 8000
```

然后访问 `http://localhost:8000/`。

## 目录结构

```
index.html   单页介绍站（全部样式内联，无 JavaScript）
NOTICE.md    第三方与素材声明
README.md    本说明
```

## 发布

推送到默认分支后由 GitHub Pages 从仓库根目录发布。发布前检查：

1. 页面中不含任何凭据、真实持仓、账户标识或内部绝对路径；
2. 所有图表标注为示意图；
3. 仓库不含原项目的历史提交、缓存或配置文件。
