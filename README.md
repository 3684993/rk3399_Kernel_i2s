# rk3399-kernel-deploy

自动化 RK3399 (NanoPC-T4) 内核编译与 sd-fuse 打包示例仓库。
将包含两个 workflow:
- build-kernel.yml：编译 kernel + u-boot + sd-fuse 打包（已修正 defconfig 使用）
- setup-test-repo.yml：可在 Actions 中运行以创建测试 repo（需 gh）

在运行之前，请把自定义补丁放到 patches/ 目录（例如 enable_i2s1.patch）。
