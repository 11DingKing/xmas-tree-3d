# 🎄 圣诞树手势交互

基于 Three.js 和 MediaPipe Hands 的 3D 手势控制圣诞树，单 HTML 文件实现。

## 运行方式

### 方式一：直接打开
双击 `frontend-user/index.html` 在浏览器中打开即可。

### 方式二：Docker 部署
```bash
docker-compose up --build -d
```
访问：http://localhost:8081

## 操作说明

### 鼠标控制
- 🖱️ 拖拽 → 旋转视角
- 👆 点击空白 → 展开/合拢切换
- 👆 点击照片 → 放大查看（散开状态下）
- 🔄 滚轮 → 缩放

### 手势控制
- ✊ 握拳 → 合拢圣诞树
- 🖐️ 张开五指 → 散开元素 + 移动旋转
- 👌 捏合 → 选择照片放大
- ↔️ 手前后移动 → 缩放视角

## 功能特性

- 🎄 3D 圣诞树场景（球体、礼物盒、糖果棍、彩带等）
- ✨ Bloom 辉光后处理效果
- ❄️ 飘雪粒子动画
- 🌙 月光夜景氛围
- ✋ MediaPipe 实时手势识别
- 📷 支持上传照片作为装饰
- 🔄 状态间平滑过渡动画

## 项目结构

```
├── frontend-user/
│   ├── index.html      # 单文件应用（所有代码）
│   ├── Dockerfile
│   └── nginx.conf
├── docker-compose.yml
└── README.md
```

## 技术栈

- Three.js（3D 渲染 + Bloom 后处理）
- MediaPipe Hands（手势识别）
- Nginx（静态文件服务）
- Docker（容器化部署）
