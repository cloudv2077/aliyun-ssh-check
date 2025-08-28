# Aliyun SSH Check

自动化SSH服务监控系统，基于GitHub Actions实现。

## 功能

- 自动监控SSH服务状态
- 多层检测机制（端口+协议）
- 智能重试策略
- 异常自动告警

## 特性

- 🔍 每5分钟自动检测
- 🔄 三次重试机制
- 📢 即时告警通知
- 🚀 支持手动触发

## 部署

推送至GitHub仓库即可自动运行。

## 监控

在Actions页面查看运行日志。

## Claude代理服务监控

### 实时监控日志
```bash
tail -f /Users/cloudv/keep-claude/proxy.log
```

### 查看错误日志
```bash
grep "ERROR" /Users/cloudv/keep-cloud/proxy.log
```

### 查看服务状态
```bash
lsof -i :8765
```
