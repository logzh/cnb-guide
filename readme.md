# cnb guide

在公司内这些年使用的比较爽的两款产品是：
- [橘子 CI](https://oci.woa.com/)，大家习惯称呼为 OCI，现更名为 云原生构建。
- [工蜂 IDE](https://git.woa.com/dashboard/ide),它是一款和 [github codespaces](https://github.com/codespaces) 类似的远程开发产品。OCI 也有远程开发功能但用的不多，因为代码都在工蜂上，自然用 工蜂 IDE 比较多。

但这些都只能在公司内使用，如果想在公司外使用，怎么办呢？

云原生构建对外的产品是 [云原生构建 CNB](https://cloud.tencent.com/product/cnb)，可以同时满足我们对 OCI 和 工蜂 IDE 的需求了。

来自官方的介绍：云原生构建（Cloud Native Build，CNB）提供代码托管、云原生构建、云原生开发、AI 代码助手和制品库等功能。基于 Docker 生态，对环境、缓存、插件进行抽象，通过声明式的语法，帮助开发者以更酷的方式构建软件。