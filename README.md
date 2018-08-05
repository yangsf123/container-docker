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

# Harbor
> https://github.com/vmware/harbor
`Features
Role based access control: Users and repositories are organized via 'projects' and a user can have different permission for images under a project.
Policy based image replication: Images can be replicated (synchronized) between multiple registry instances, with auto-retry on errors. Great for load balancing, high availability, multi-datacenter, hybrid and multi-cloud scenarios.
Vulnerability Scanning: Harbor scans images regularly and warns users of vulnerabilities.
LDAP/AD support: Harbor integrates with existing enterprise LDAP/AD for user authentication and management.
Image deletion & garbage collection: Images can be deleted and their space can be recycled.
Notary: Image authenticity can be ensured.
Graphical user portal: User can easily browse, search repositories and manage projects.
Auditing: All the operations to the repositories are tracked.
RESTful API: RESTful APIs for most administrative operations, easy to integrate with external systems.
Easy deployment: Provide both an online and offline installer.`

相关文章：
  https://mp.weixin.qq.com/s/2vXrfkzpEK032dnPqNPtkQ
  https://mp.weixin.qq.com/s/4VRcRPXHhoaLbCtzRR3IDQ
  https://mp.weixin.qq.com/s/4VRcRPXHhoaLbCtzRR3IDQ
  https://mp.weixin.qq.com/s/8o8YMRjNpwsBjyiQR7PF3A
  https://mp.weixin.qq.com/s/tlk-EDA82cf5BHT2tT5L-w
  https://mp.weixin.qq.com/s/Tj7XGo023h3zXOpxDtkNMQ

# Notary
> https://github.com/theupdateframework/notary
可信容器映像服务：Notary 是云原生计算基金会 CNCF (Cloud Native Computing Foundation) 的官方项目，为容器映像提供数字签名保护，以防止对于容器映像的恶意篡改。该功能打开之后，只有经过数字签名的映像才能被部署到 PKS 集群里去运行。

# Clair
> https://github.com/coreos/clair
