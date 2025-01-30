# 需求分析智能体

这是一个基于大语言模型的通用需求分析工具，可以帮助您：
- 分析各类项目需求
- 提供专业建议和建设性意见
- 基于"拆推评算"框架进行深入分析
- 支持交互式对话，解答疑问

## 应用场景

适用于各类项目的需求分析，例如：
- 软件开发项目
- 产品规划设计
- 业务流程优化
- 系统架构设计
- 创业项目评估
等

## 使用方法

1. 填写项目信息：
   - 项目名称
   - 行业领域
   - 项目阶段
   - 项目描述

2. 点击"分析需求"按钮，系统会基于"拆推评算"框架生成分析报告

3. 您可以继续提问，与系统进行深入对话，获取更多专业建议

## 示例项目

本项目以"天枢云住"为示例，展示了智能体如何分析房地产行业的项目需求。您可以参考这个示例，将分析框架应用到自己的项目中。

## 在线体验

访问：https://superhui1975.github.io/customer-needs

## 特色功能

- 基于"拆推评算"的专业分析框架
- 交互式对话，深入探讨
- 实时响应，即时反馈
- 支持多领域项目分析
- 简洁直观的操作界面

## 安全提示

- 请勿在项目描述中包含敏感信息
- 建议在正式使用前进行测试评估
- 分析结果仅供参考，关键决策请结合实际情况

## 后续优化方向

1. 扩展更多行业分析模板
2. 优化分析框架
3. 提供报告导出功能
4. 支持多轮对话历史
5. 添加更多场景示例

## 部署方式

### 1. 本地开发环境

1. 克隆项目到本地
```bash
git clone [your-repository-url]
cd [repository-name]
```

2. 安装依赖
```bash
pip install -r requirements.txt
```

3. 配置环境变量
创建`.env`文件并添加以下内容：
```
DEEPSEEK_API_KEY=your_api_key_here
```

4. 启动后端服务
```bash
python app.py
```

5. 访问应用
打开浏览器访问：`http://localhost:5000`

### 2. 生产环境部署

#### 方式一：使用 GitHub Pages（前端）+ Vercel（后端）

1. 前端部署（GitHub Pages）：
   - Fork 本仓库
   - 进入仓库设置 (Settings)
   - 在 Pages 设置中选择 main 分支
   - 等待部署完成

2. 后端部署（Vercel）：
   - 注册 [Vercel](https://vercel.com) 账号
   - 导入后端代码仓库
   - 配置环境变量（DEEPSEEK_API_KEY）
   - 部署项目
   - 获取生产环境API地址

3. 更新前端配置：
   - 修改 `index.html` 中的 `API_BASE_URL` 为 Vercel 提供的地址
   - 提交更改并等待 GitHub Pages 重新部署

#### 方式二：使用 Docker

1. 构建镜像
```bash
docker build -t demand-analysis .
```

2. 运行容器
```bash
docker run -d -p 5000:5000 -e DEEPSEEK_API_KEY=your_api_key_here demand-analysis
```

## 技术栈

- 前端：HTML + CSS + JavaScript
- UI框架：Bootstrap 5
- Markdown渲染：marked.js
- 后端：Python Flask
- API：Deepseek Chat API

## 贡献指南

欢迎提交 Issue 和 Pull Request 来帮助改进项目。

## 许可证

MIT License