# sa-test

Super Agent 测试仓库。

## 使用说明

### 获取仓库

```bash
git clone https://github.com/fengrussell/sa-test.git
cd sa-test
```

### 查看内容

仓库当前仅包含本 README 文件，用于验证仓库读写与 PR 流程：

```bash
ls
cat README.md
```

### 提交改动

1. 从 `main` 创建分支，分支名建议使用 `agent/<简短描述>`：

   ```bash
   git checkout main
   git pull origin main
   git checkout -b agent/<简短描述>
   ```

2. 修改文件后提交：

   ```bash
   git add README.md
   git commit -m "describe your change"
   git push origin agent/<简短描述>
   ```

3. 在 GitHub 上以 `main` 为目标分支创建 Pull Request，等待评审；合并由维护者完成，不要自行合并。

### 分支约定

- `main`：稳定分支，直接推送前需确认。
- `agent/*`：自动化或协作分支，通过 PR 合入 `main`。
