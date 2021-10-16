# 파드(Pod)



1. 쿠버네티스의 실행 최소 단위
2. 상태변경이 있을 경우 create보다는 apply로 사용하는 습관





#### 명령어



```shell
kubectl get pods -o wide

kubectl run nginx --image=nginx                     # Run pod nginx and write its spec into a file called pod.yaml
--dry-run=client -o yaml > pod.yaml


```



replicas 교체 명령어

```shell
sed -i -e 's|replicas: 3|replicas: 4|' sample-rs.yamls
```

