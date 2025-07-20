# 如何在CNB中使用 codespaces 环境

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
      env:
        CNB_WELCOME_EXECUTE_COMMAND: go version
      stages:
        - name: ls
          script: ls -al
        - name: go version
          script: go version
        - name: node v
          script: node -v
        - name: python v
          script: python --version
```