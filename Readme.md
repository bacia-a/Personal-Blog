# 🌸 樱花主题个人博客

一个基于 **Vue3 + Django** 的个人博客项目，具有精美的樱花飘落动画效果和完整的内容管理系统。

![樱花博客](https://img.shields.io/badge/Vue-3.3.4-brightgreen) ![Django](https://img.shields.io/badge/Django-5.2.7-green) ![License](https://img.shields.io/badge/license-MIT-blue)

## ✨ 项目特点

- 🌸 **樱花主题** - 独特的樱花飘落动画效果
- 🎮 **游戏展示** - 游戏收藏展示系统，支持截图画廊
- 📺 **动漫展示** - 动漫收藏展示系统，支持截图画廊
- 📱 **响应式设计** - 完美适配PC、平板、手机
- 🎨 **精美UI** - 流畅的交互动画和现代化设计
- 🔧 **易于管理** - Django Admin后台，便捷的内容管理

## 🚀 快速开始

### 环境要求

- Python 3.9+
- Node.js 16+

### 1. 克隆项目

```bash
git clone https://github.com/bacia-a/Personal-Blog.git
```

### 2. 后端配置

```bash
cd backend

# 安装依赖
pip install -r requirements.txt

# 数据库迁移
python manage.py migrate

# 创建管理员账户
python manage.py createsuperuser

# 启动后端服务
python manage.py runserver
```

后端服务：`http://127.0.0.1:8000`  
管理后台：`http://127.0.0.1:8000/admin`

### 3. 前端配置

```bash
cd frontend

# 安装依赖
npm install

# 启动开发服务器
npm run dev
```

前端服务：`http://localhost:5173`

## 📦 功能模块

### 核心功能

| 模块 | 功能描述 |
|------|---------|
| 🖼️ **轮播图** | 全屏轮播展示，自动/手动切换 |
| 👤 **个人信息** | 头像、简介 |
| 💼 **作品展示** | 作品集展示，支持外链跳转 |
| 🎯 **爱好展示** | 标签页切换展示游戏、动漫 |

### 扩展功能

#### 🎮 游戏模块
- 游戏卡片网格展示
- 5星评分系统
- 游玩时长显示
- 详情弹窗
- 游戏截图画廊

#### 📺 动漫模块
- 动漫海报墙展示
- 5星评分系统
- 年份/状态标签
- 详情弹窗
- 精彩截图画廊

## 🎨 技术栈

### 前端
- **Vue 3.3** - 渐进式JavaScript框架
- **Vue Router 4** - 官方路由管理
- **Axios** - HTTP客户端
- **Tailwind CSS** - 实用优先的CSS框架
- **Anime.js** - 轻量级动画库
- **Vite** - 下一代前端构建工具

### 后端
- **Django 5.2** - Python Web框架
- **Django REST Framework** - RESTful API工具包
- **SQLite** - 轻量级数据库
- **Pillow** - Python图像处理库


## 🔧 后台管理

访问 `http://127.0.0.1:8000/admin` 进入管理后台。

### 管理功能
- ✅ 个人信息管理
- ✅ 轮播图管理
- ✅ 作品管理
- ✅ 游戏管理（含截图）
- ✅ 动漫管理（含截图）

## 🚢 部署

### 前端部署
```bash
cd frontend
npm run build
# 将 dist 目录部署到静态服务器
```

### 后端部署
```bash
# 修改 settings.py
DEBUG = False
ALLOWED_HOSTS = ['your-domain.com']

# 使用 Gunicorn
pip install gunicorn
gunicorn blog_backend.wsgi:application
```

