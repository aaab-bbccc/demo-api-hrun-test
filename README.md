# HttpRunner 接口自动化测试项目
> 软件测试实战项目，基于HttpRunner v4实现接口自动化，适合测试岗位简历项目

## 📌 项目简介
使用HttpRunner搭建接口自动化测试框架，完成接口请求、参数提取、业务关联、结果断言，实现登录token跨用例传递，自动化校验接口返回状态码与业务返回JSON。

## 🛠 技术栈
- 框架：HttpRunner v4
- 脚本格式：YAML测试用例
- 版本管理：Git + GitHub
- 辅助：Postman、AI辅助用例设计与报错定位

## ✨ 项目功能
1. GET请求接口测试、POST-JSON请求接口测试
2. extract变量提取：提取登录接口返回的token，传递给后续业务接口
3. validate断言：校验响应状态码+返回体业务字段，不仅仅判断200
4. 批量执行测试用例，自动生成测试报告
5. .gitignore配置，忽略虚拟环境、缓存文件，减少仓库冗余

## 📂 目录说明
- testcases：YAML测试用例目录，包含demo.yml、post_demo.yml、token_demo.yml
- reports：自动化测试报告输出目录
- .gitignore：git忽略文件配置

## 🚀 运行方式
```bash
# 安装依赖
pip install httprunner
# 执行测试用例
hrun testcases/token_demo.yml
