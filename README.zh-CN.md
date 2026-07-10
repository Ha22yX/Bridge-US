<div align="center">
  <h1>Bridge US</h1>
  <p>一个早期 Flask 社区原型，帮助国际学生分享赴美初期的实用经验。</p>

  <p>
    <a href="README.md">English</a>
    &middot;
    <a href="https://github.com/Ha22yX/Bridge-US-V2">Bridge-US V2</a>
    &middot;
    <a href="#快速开始">快速开始</a>
    &middot;
    <a href="#核心能力">核心能力</a>
    &middot;
    <a href="#技术栈">技术栈</a>
  </p>

  <p>
    <img alt="Python: Flask" src="https://img.shields.io/badge/Python-Flask-3776AB?style=for-the-badge&logo=python&logoColor=white" />
    <img alt="Community: prototype" src="https://img.shields.io/badge/Community-prototype-287866?style=for-the-badge" />
    <img alt="Version: v1" src="https://img.shields.io/badge/Version-v1-6b7f73?style=for-the-badge" />
  </p>
</div>

<p align="center">
  <img src=".github/assets/readme-hero.svg" alt="Bridge US 项目概览图" width="100%" />
</p>

<p align="center">
  <img src="docs/pic/image.png" alt="Bridge US prototype screenshot" width="100%" />
</p>

## 项目概览

Bridge US v1 是国际学生社区想法的第一版可运行原型。

它刻意保持简单：服务端渲染页面、SQLite 内容流程，以及通过审核后公开的帖子机制。

## 核心能力

- 围绕到达、住房、交通、饮食、生活手续和安全等主题的分类经验帖。
- 注册/登录、发帖和后台审核队列。
- 仅公开已审核内容，形成基础可信流程。
- `docs/` 中保留产品规划文档和截图。
- 与 Bridge-US-V2 的关系清晰：V2 是更完整的独立重写。

## 工作方式

1. 用户按分类浏览实用经验帖。
2. 注册用户提交自己的经验内容。
3. 管理员审核新内容后再公开。
4. 仓库记录了 V2 重写前的早期产品方向。

## 快速开始

可以用下面的命令在本地运行项目。

```bash
git clone https://github.com/Ha22yX/Bridge-US.git
cd Bridge-US
python -m venv .venv
.venv\Scripts\activate
pip install -r requirements.txt
python app.py
```

打开 `http://127.0.0.1:5000`。这个仓库是 V1 原型；更完整的产品架构请看 V2。

## 配置项

| 项目 | 作用 |
| --- | --- |
| `SECRET_KEY` | 部署前为 Flask 会话设置密钥。 |
| SQLite 数据库 | 本地原型存储；真实使用前应备份。 |
| 后台审核 | 通过审核队列控制公开内容。 |
| V2 迁移 | 新增复杂功能前建议优先查看 Bridge-US-V2。 |

## 技术栈

| 层级 | 技术 | 作用 |
| --- | --- | --- |
| 后端 | Flask | 路由、模板和会话。 |
| 数据 | SQLite | 原型数据库。 |
| 前端 | Jinja, CSS | 服务端渲染社区页面。 |
| 文档 | Markdown | 产品规划和路线说明。 |

## 项目结构

```text
app.py                  Flask 应用
db.py                   数据库辅助逻辑
templates/              社区和后台页面
static/                 CSS 与静态资源
docs/                   规划文档和截图
```

## 项目状态

早期原型。Bridge-US 和 Bridge-US-V2 目标相同，但彼此独立；V2 更完整。

## 相关项目

- [Bridge-US V2](https://github.com/Ha22yX/Bridge-US-V2) - 相关版本/配套项目。

## 许可证

当前仓库尚未声明项目级开源许可证；公开复用或分发前建议先补充 License。
