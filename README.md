# 🌐 Velixox - AS123456 网络介绍首页

这是一个专业的网络基础设施服务商介绍网站，展示 Velixox 的自治系统信息（AS123456）和全球网络服务。

## ✨ 功能特性

- 📋 **网络基本信息展示**
  - AS号码：AS123456
  - 网络类型、BGP协议版本
  - IPv4/IPv6双栈支持
  - 可用IP地址段数
  - 国际互联点数
  - 技术规格展示

- 🌍 **全球服务范围**
  - 欧洲服务（12+ 国家，3个数据中心）
    - 枢纽：阿姆斯特丹、伦敦、法兰克福
    - 带宽：300+ Gbps
  - 亚太服务（15+ 国家，3个数据中心）
    - 枢纽：新加坡、东京、香港
    - 带宽：350+ Gbps
  - 美国服务（28+ 州，2个数据中心）
    - 枢纽：纽约、硅谷
    - 带宽：350+ Gbps

- 🎨 **现代化设计**
  - 响应式布局
  - 美观的渐变背景
  - 流畅的动画效果
  - 完整的移动端适配

- 📱 **用户友好**
  - 清晰的信息层级
  - 快速导航
  - 专业的视觉设计

## 🚀 快速开始

### 本地开发

```bash
# 克隆存储库
git clone https://github.com/hyhx-ai/hedox-asn.git
cd hedox-asn

# 启动本地服务器
python -m http.server 8000

# 或使用 Node.js
npx http-server

# 访问 http://localhost:8000
```

### Cloudflare Pages 部署

1. **连接 GitHub 仓库**
   - 访问 https://pages.cloudflare.com
   - 授权 Cloudflare 访问你的 GitHub
   - 选择 `hedox-asn` 仓库

2. **配置构建设置**
   - 构建命令：（留空，因为是静态网站）
   - 输出目录：`/`

3. **自动部署**
   - Cloudflare 会自动部署到：`https://hedox-asn.pages.dev`
   - 每次 push 到 main 分支都会自动重新部署

### Docker 部署

```dockerfile
FROM nginx:alpine
COPY . /usr/share/nginx/html/
EXPOSE 80
CMD ["nginx", "-g", "daemon off;"]
```

```bash
# 构建镜像
docker build -t velixox-asn .

# 运行容器
docker run -p 80:80 velixox-asn

# 访问 http://localhost
```

## 📁 项目结构

```
hedox-asn/
├── index.html        # 主页面
├── style.css        # 样式文件
├── README.md        # 本文件
└── .gitignore       # Git 忽略配置
```

## 📝 修改内容

### 修改 ASN 号码
编辑 `index.html`，查找并替换所有 `AS123456` 和 `123456`：

```html
<!-- 将此处替换为你的 ASN -->
<span class="asn-badge">AS123456</span>
<div class="asn-large">AS123456</div>
```

### 修改组织名称
编辑 `index.html`，替换所有 `Velixox` 为你的组织名称：

```html
<h1>🌐 Velixox</h1>
<h1>Velixox</h1>
<p class="hero-subtitle">全球高效网络基础设施服务商</p>
```

### 修改服务范围信息
编辑 `index.html` 中的 `.coverage-card` 部分：

```html
<div class="coverage-stat">
    <span class="stat-label">覆盖国家:</span>
    <span class="stat-value">12+</span>
</div>
```

### 修改样式颜色
编辑 `style.css` 中的 CSS 变量：

```css
:root {
    --primary-color: #2563eb;      /* 主要颜色 */
    --secondary-color: #1e40af;    /* 次要颜色 */
    --accent-color: #0ea5e9;       /* 强调颜色 */
}
```

### 修改联系方式
编辑 `index.html` 中的联系卡片部分：

```html
<div class="contact-card">
    <div class="contact-icon">📧</div>
    <h3>电子邮件</h3>
    <p>support@velixox.com</p>
</div>
```

## 🌐 在线访问

部署后可通过以下地址访问：
- **Cloudflare Pages**: `https://hedox-asn.pages.dev`
- **自定义域名**：在 Cloudflare 管理面板配置

## 🎯 SEO 优化

网站已包含以下 SEO 优化：
- Meta 描述和关键词
- 语义化 HTML 结构
- 响应式设计（移动端友好）
- 快速加载时间
- 无外部依赖

## 🔧 浏览器兼容性

- ✅ Chrome/Edge (最新版)
- ✅ Firefox (最新版)
- ✅ Safari (最新版)
- ✅ Mobile Safari (iOS 12+)
- ✅ Chrome Mobile (Android 5+)

## 📚 技术栈

- **HTML5** - 语义化标记
- **CSS3** - 现代样式和布局
- **纯JavaScript** - 无框架依赖
- **Cloudflare Pages** - 部署平台

## 🔐 许可证

MIT License - 自由使用和修改

## 🤝 支持

如有问题或建议，欢迎提交 Issue 或 Pull Request。

---

**Velixox AS123456** - 全球网络基础设施服务商