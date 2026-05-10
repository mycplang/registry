# CP 语言官方包注册表

CP语言的中文包管理器「包」默认注册表。

### 使用

```bash
包 注册表 https://raw.githubusercontent.com/cplang/registry/main/index.json
包 安装 math
包 安装 string
```

### 贡献包

1. Fork 本仓库
2. 在 packages/ 下新建目录，放入 index.cp
3. 更新 index.json 添加条目
4. 提 PR

### 包结构

```
packages/
  包名/
    index.cp    ← 包入口文件（导出所有函数）
```

包的 index.cp 中定义的所有 `函数` 会自动被 `导入 包名` 暴露给调用方。
