---
home: true
heroText: 《Pomelo's Blog 食用指南》
# actionText: 立刻进入 →
# actionLink: /web/
# bannerBg: auto # auto => 网格纹背景(有bodyBgImg时无背景)，默认 | none => 无 | '大图地址' | background: 自定义背景样式       提示：如发现文本颜色不适应你的背景时可以到palette.styl修改$bannerTextColor变量
---

## 1、查看资源申请情况
```bash
kubectl describe node mxpoc-m01（当前的命名空间）
```

## 2、确认 Hami 调度组件的服务暴露情况（查看 Kubernetes 系统组件暴露了哪些 Service）
```bash
kubectl get svc -n kube-system
```
```bash
curl 10.62.242.110:31993/metrice
```

## 3、查看创建pod节点的yaml文件
```bash
kubectl get pods pod名 -n 命名空间 -oyaml
```
