# agent.No1
## 项目简介
基于 AstrBot 搭建的学习辅助 QQ Bot。
项目部署于 Linux 云服务器
集成 DeepSeek 大模型，RAG知识库检索，联网搜索及群管理，小游戏等功能。
本人主要负责部署，配置，调试与维护工作。
## 功能
已接入功能

- RAG知识库问答
- 联网搜索
- 每日单词推送
- 插件扩展
- Q群管理（监控对话中是否出现屏蔽词，入群防人机验证...)
- 活跃气氛小游戏
- 其中部分功能基于 AstrBot 插件生态实现。
## 技术栈

### 开发环境
- Python
- Linux
- Ubuntu Server
### AI能力
- DeepSeek API
- text-embedding-v3
- Qwen3-Reranker
### 框架
- AstrBot
### 工具
GitHub
## 项目截图
对话：
<img width="2559" height="1217" alt="屏幕截图 2026-06-22 235844" src="https://github.com/user-attachments/assets/93b87969-de48-40a1-bb5a-92f109297197" />
<img width="1989" height="1291" alt="屏幕截图 2026-06-22 235900" src="https://github.com/user-attachments/assets/8e64badb-b87d-4d2b-bfed-96b15c8541d1" />
<img width="2003" height="1242" alt="屏幕截图 2026-06-22 235910" src="https://github.com/user-attachments/assets/9e662472-ecc8-42de-8541-7de1aa821959" />
日志：
<img width="2313" height="1564" alt="屏幕截图 2026-06-22 235807" src="https://github.com/user-attachments/assets/ea5c43f8-c654-4a63-81c6-ff390c739bab" />
<img width="2518" height="1595" alt="屏幕截图 2026-06-22 235817" src="https://github.com/user-attachments/assets/dccab48b-37be-4350-9547-e793d6306974" />
<img width="2559" height="1580" alt="屏幕截图 2026-06-22 235830" src="https://github.com/user-attachments/assets/35fcd4f0-3dc4-4228-9b1b-eef01a1788d1" />

## 遇到的问题

### 问题1：模型出现幻觉

原因：知识库召回不足。

解决：优化检索配置并增加重排序模型。

---

### 问题2：插件无法触发

原因：metadata.yaml 配置错误。

解决：检查插件结构并重新加载。

---

### 问题3：API调用失败

原因：配置错误。

解决：重新检查接口参数与模型配置。

### 问题4：模型出现幻觉

原因：RAG召回不足,Prompt约束不够

解决：调整检索参数,增加重排序模型并优化Prompt
### 问题5：插件无法触发

原因：metadata.yaml配置错误

解决：检查文件更改后重新加载插件。
## 开发收获
在项目搭建过程中学习并实践了：
- Linux 云服务器部署
- Python 基础开发
- GitHub 项目管理
- Prompt 工程基础
- RAG 知识库原理
- 向量检索与重排序
- API 调用与模型配置
- AstrBot 插件管理与调试
- LLM 工作原理与幻觉问题分析
## 项目成果
- 成功部署到云服务器且成功运行至今
- 支持多人使用
- 实现知识库问答
- 开发自定义插件
## 我的工作
本项目基于 AstrBot 开源框架搭建
本人主要负责：
- 云服务器部署
- 模型API配置
- 知识库接入
- 插件安装与测试
- Bot日常维护与优化
