# 灵镜创作工作台前端

Lingjing Creative Studio 的 Web 创作工作台，基于 Next.js 与 React，提供创作流程、任务进度、素材预览及模型设置。

## 本地启动

从项目根目录“灵镜创作工作台”进入前端目录：

```bash
cd lingjing/lingjing/frontend
npm ci
npm run dev
```

访问 http://localhost:3000。

前端会将 API 请求转发到 http://127.0.0.1:8000，因此需要在另一个终端启动后端。从项目根目录执行：

```bash
cd lingjing/lingjing/backend
venv/bin/python api_server.py
```

如果使用 uv 管理后端环境，也可执行 `uv run python api_server.py`。

## 生产构建

在前端目录执行：

```bash
npm run build
npm start
```

## 品牌资源

- `public/logo.svg`：页面 Logo。
- `app/icon.svg`：浏览器标签图标。
- `app/layout.tsx`：页面标题与说明。

完整安装、模型配置与产物目录见[项目 README](../../../README.md)。
