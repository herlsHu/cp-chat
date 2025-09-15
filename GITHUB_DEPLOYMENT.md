
# GitHub Pages 部署说明

## 1. 推送代码到GitHub

```bash
git add .
git commit -m "Deploy static version with DeepSeek API"
git push origin main
```

## 2. 设置GitHub Secrets

在GitHub仓库设置中添加以下Secrets:

- `DEEPSEEK_API_KEY`: sk-738628ee54124893b04549c845689b9a
- `API_BASE_URL`: https://6b2miwy3n5.ap-northeast-1.awsapprunner.com
- `API_TOKEN`: eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VySWQiOiI2OGI5NjYyYjljYzVlMjZmNjBjNTk1YTAiLCJ1c2VybmFtZSI6InRlc3R1c2VyX3Byb2R1Y3QiLCJleHAiOjE3NTk1NzI3Nzl9.iP6znTApaixpqVux5YAIHG6DCbU7Y-ocYQjMy9iP9l4
- `CHARACTER_ID`: 68b96da8d1cebe8b32c595a0
- `USER_ID`: 68b9662b9cc5e26f60c595a0
- `DEVICE_ID`: PC-LOCAL

## 3. 启用GitHub Pages

1. 进入仓库设置
2. 找到 "Pages" 部分
3. 选择 "GitHub Actions" 作为源
4. 等待部署完成

## 4. 访问地址

部署完成后，你的应用将可以通过以下地址访问:
- `https://你的用户名.github.io/仓库名`

## 5. 功能特性

- ✅ 角色选择界面
- ✅ 聊天对话功能
- ✅ 图片上传和描述
- ✅ 无料卡生成
- ✅ 移动端适配
- ✅ 国内直接访问

## 6. 注意事项

- 所有API调用都在前端进行
- API密钥会暴露在前端代码中
- 确保图片API支持CORS跨域访问
- 建议使用HTTPS部署

## 7. 故障排除

如果遇到问题，请检查:
1. GitHub Secrets是否正确设置
2. 仓库是否启用了GitHub Pages
3. 构建日志是否有错误
4. 浏览器控制台是否有错误信息
