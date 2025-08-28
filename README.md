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

### 服务信息
- **端口**: 8765
- **服务**: Claude API代理服务器
- **进程**: python3 1proxy.py
- **日志位置**: `/Users/cloudv/keep-claude/proxy.log`

### 日志监控命令

#### 实时监控日志
```bash
tail -f /Users/cloudv/keep-claude/proxy.log
```

#### 查看最近100行日志
```bash
tail -100 /Users/cloudv/keep-claude/proxy.log
```

#### 查看错误日志
```bash
grep -E "(ERROR|WARNING|CRITICAL)" /Users/cloudv/keep-claude/proxy.log
```

#### 查看服务状态
```bash
lsof -i :8765
```

### 服务特点
- 🔄 自动API密钥轮换
- 🛡️ 安全的系统级密钥管理
- 🚀 高并发请求处理
- 📊 详细的请求日志记录
- 🔁 智能错误重试机制

