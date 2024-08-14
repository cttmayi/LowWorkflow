# Flowise - 轻松构建 LLM 应用程序

## 👨‍💻 开发者

Flowise 在一个单一的代码库中有 3 个不同的模块。

- `server`：用于提供 API 逻辑的 Node 后端
- `ui`：React 前端
- `components`：第三方节点集成

### 先决条件

- 安装 [PNPM](https://pnpm.io/installation)
  
    ```bash
    npm i -g pnpm
    ```

### 设置

1. 克隆仓库

    ```bash
    git clone https://github.com/cttmayi/LowWorkflow.git
    ```

2. 进入仓库文件夹

    ```bash
    cd LowWorkflow
    ```

3. 安装所有模块的依赖：

    ```bash
    pnpm install
    ```

4. 构建所有代码：

    ```bash
    pnpm build
    ```

5. 启动应用：

    ```bash
    pnpm start
    ```

    现在可以在 [http://localhost:3000](http://localhost:3000) 访问应用

6. 用于开发构建：

    - 在 `packages/ui` 中创建 `.env` 文件并指定 `VITE_PORT`（参考 `.env.example`）
    - 在 `packages/server` 中创建 `.env` 文件并指定 `PORT`（参考 `.env.example`）
    - 运行

        ```bash
        pnpm dev
        ```

    任何代码更改都会自动重新加载应用程序，访问 [http://localhost:8080](http://localhost:8080)

## 🔒 认证

要启用应用程序级身份验证，在 `packages/server` 的 `.env` 文件中添加 `FLOWISE_USERNAME` 和 `FLOWISE_PASSWORD`：

```
FLOWISE_USERNAME=user
FLOWISE_PASSWORD=1234
```

## 🌱 环境变量

Flowise 支持不同的环境变量来配置您的实例。您可以在 `packages/server` 文件夹中的 `.env` 文件中指定以下变量。了解更多信息，请阅读[文档](https://github.com/FlowiseAI/Flowise/blob/main/CONTRIBUTING.md#-env-variables)

## 📖 文档

[Flowise 文档](https://docs.flowiseai.com/)

## 📄 许可证

此代码库中的源代码在[Apache License Version 2.0 许可证](LICENSE.md)下提供。
