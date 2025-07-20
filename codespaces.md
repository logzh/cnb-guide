# 如何在CNB中使用 codespaces 环境

[CNB 自定义开发环境](https://docs.cnb.cool/zh/workspaces/custom-dev-env.html)

.cnb.yml 中配置 codespaces 环境镜像即可

```
$:
  vscode:
    - docker:
        image: mcr.microsoft.com/devcontainers/universal
        #image: mcr.microsoft.com/devcontainers/go:1.24
      services:
        - vscode
        - docker
      stages:
        - name: go version
          script: go version
        - name: node v
          script: node -v
        - name: python v
          script: python --version
```