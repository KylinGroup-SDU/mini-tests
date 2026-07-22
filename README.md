# mini-tests
Mini-tests for quantum-chemistry graduate student

## 环境配置

Arch Linux 需要安装 OpenBLAS 并将 include 路径加入编译环境：

```bash
# 安装依赖
sudo pacman -S openblas

# 加载环境变量后同步项目
source .env && uv sync
```

> `.env` 中设置了 `CPATH=/usr/include/openblas`，供 zquatev 编译时查找 `cblas.h`。
