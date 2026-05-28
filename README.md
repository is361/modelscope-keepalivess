# ModelScope 空间保活

## 使用步骤

### 1. 创建 GitHub 仓库
```bash
cd modelscope-keepalive
git init
git add .
git commit -m "init: ModelScope keep-alive"
git remote add origin <你的仓库地址>
git push -u origin main
```

### 2. 修改 keepalive.yml
把 `SPACE_URL` 换成你魔搭空间的实际地址。

魔搭空间的 URL 格式通常是：
- `https://modelscope.cn/studios/<用户名>/<空间名>`
- 如果有自定义域名，用你的实际域名

### 3. GitHub Actions 自动运行
推送后，Actions 会自动每 5 分钟 ping 一次你的空间。

⚠️ **注意**：GitHub Actions 对公开仓库免费无限使用，私有仓库每月有限额（2000 分钟）。

---

## 生效验证
1. 去仓库的 Actions 标签页确认 workflow 运行成功
2. 等 30 分钟后检查魔搭空间是否还醒着