# pnpm 章节

pnpm 是前端目前最前沿的包管理工具，具有以下优点

1. 安装速度快，resolve 和 fetch 两个流程相结合

2. 节省空间，从全局中心化的 store 中 clone 或者 hardlink 文件，来降低磁盘空间的占用

3. 严格，通过 symlink 提供非扁平化的 `node_modules` 结构，每个包只可 resolve 到自己 `package.json` 中声明的依赖

4. monorepo 支持，提供 workspace 协议来 symlink 其他子项目，或使用 --filter 来批量调用脚本等
