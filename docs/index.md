---
home: true
# heroImage: /img/web.png
heroText: Pomelo's Blog
tagline: 我愿用我三生的烟火,换你一世的迷离
# actionText: 立刻进入 →
# actionLink: /web/
# bannerBg: auto # auto => 网格纹背景(有bodyBgImg时无背景)，默认 | none => 无 | '大图地址' | background: 自定义背景样式       提示：如发现文本颜色不适应你的背景时可以到palette.styl修改$bannerTextColor变量

# features: # 可选的
#   - title: 技术笔记
#     details: 用来沉淀 可复用、可查阅、可系统化 的内容
#     link: /web/ # 可选
#   - title: 工程实践
#     details: 把「会」变成「做过」
#     link: /ui/
#   - title: 学习路线
#     details: 当前阶段的探索方向
#     link: /technology/
# 文章列表显示方式: detailed 默认，显示详细版文章列表（包括作者、分类、标签、摘要、分页等）| simple => 显示简约版文章列表（仅标题和日期）| none 不显示文章列表
# postList: detailed
# simplePostListLength: 10 # 简约版文章列表显示的文章数量，默认10。（仅在postList设置为simple时生效）
# hideRightBar: true # 是否隐藏右侧边栏
---

# 沐曦1-k8s

### 1、查看资源申请情况
```bash
kubectl describe node mxpoc-m01（当前的命名空间）
```

### 2、确认 Hami 调度组件的服务暴露情况（查看 Kubernetes 系统组件暴露了哪些 Service）
```bash
kubectl get svc -n kube-system
```
```bash
curl 10.62.242.110:31993/metrice
```

### 3、查看创建pod节点的yaml文件
```bash
kubectl get pods pod名 -n 命名空间 -oyaml
```
