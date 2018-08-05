# container-docker

## Docker背后的内核知识
namespace资源隔离

namespace   系统调用参数    隔离内容
UTS       CLONE_NEWUTS    主机名与域名
IPC       CLONE_NEWIPC    信号量、消息队列和共享内存
PID       CLONE_PID       进程编号
Network   CLONE_NEWNET    网络设备、网络栈、端口
Mount     CLONE_NEWNS     挂载点（文件系统）
User      CLONE_NEWUSER   用户和用户组





# Docker Registry v2 authentication
> https://github.com/docker/distribution/blob/master/docs/spec/auth/token.md

# Notary
> https://github.com/theupdateframework/notary
