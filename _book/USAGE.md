# PandaTool帮助文档使用说明

## 项目概述

这是一个基于 HonKit (GitBook) 的文档项目，包含了 PandaTool 一键发币工具的完整使用指南。

## 已创建的文件

- `package.json` - Node.js 项目配置文件
- `package-lock.json` - 依赖锁定文件
- `book.json` - HonKit/GitBook 配置文件

## 使用方法

### 1. 安装依赖

```bash
npm install
```

### 2. 启动开发服务器

```bash
npm run serve
```

服务将在 `http://localhost:4000` 启动，支持实时预览和热重载。

### 3. 构建静态网站

```bash
npm run build
```

构建完成后，静态文件将生成在 `_book` 目录中。

### 4. 导出为其他格式

```bash
# 导出为 PDF
npm run pdf

# 导出为 EPUB
npm run epub

# 导出为 MOBI
npm run mobi
```

## 项目结构

```
├── README.md              # 项目首页
├── SUMMARY.md             # 目录结构
├── navigation.md          # 工具导航
├── contact.md             # 联系我们
├── price.md               # 服务费用
├── createtoken/           # 代币创建相关文档
├── sol/                   # Solana链相关文档
├── ton/                   # TON链相关文档
├── sui/                   # Sui链相关文档
├── tron/                  # 波场链相关文档
├── presale/               # 预售相关文档
├── bridge/                # 跨链桥相关文档
├── tools/                 # 操作工具相关文档
├── practical-information/ # 实用信息
├── question/              # 常见问题
├── declaration/           # 相关声明
└── Web3词典/              # Web3词典
```

## 注意事项

1. 项目使用 HonKit 4.0.0 版本
2. 文档语言设置为中文 (zh-hans)
3. 某些文档中可能包含 GitBook 特有的语法，如果构建时出现错误，可能需要手动修复这些语法
4. 建议使用 Node.js 14.0.0 或更高版本

## 故障排除

### 构建失败

如果构建时出现模板渲染错误，通常是因为文档中包含了 HonKit 不支持的语法。常见的错误包括：

- `{% hint %}` 标签
- `{% embed %}` 标签
- 其他 GitBook 特有的语法

解决方法：
1. 手动编辑相关文档，移除或替换不支持的语法
2. 或者安装相应的插件来支持这些语法

### 服务启动失败

如果服务无法启动，请检查：
1. 端口 4000 是否被占用
2. Node.js 版本是否符合要求
3. 依赖是否正确安装

## 技术支持

如有问题，请参考：
- [HonKit 官方文档](https://github.com/honkit/honkit)
- [GitBook 文档](https://docs.gitbook.com/)

---

**项目状态**: ✅ 已配置完成，可以正常使用
**最后更新**: 2024年
