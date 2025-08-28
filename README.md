# 服务监控系统

## SSH 监控服务

自动化SSH服务监控系统，基于GitHub Actions实现。

### 功能特性
- 🔍 每5分钟自动检测SSH服务状态
- 🔄 智能三次重试机制
- 📢 实时异常告警通知
- 🚀 支持手动触发检测
- 🛡️ 多层检测机制（端口+协议验证）

### 部署使用
1. 推送代码至GitHub仓库
2. 自动启用Actions工作流
3. 在Actions页面查看监控日志

## Claude API 代理服务

运行在8765端口的Claude API代理服务器。

### 快速监控
```bash
# 实时日志监控
tail -f /Users/cloudv/keep-claude/proxy.log

# 查看错误信息
grep "ERROR" /Users/cloudv/keep-claude/proxy.log

# 检查服务状态
lsof -i :8765
```

### 服务特点
- 🔄 自动API密钥轮换
- 🛡️ 系统级安全管理
- 🚀 高并发处理能力
