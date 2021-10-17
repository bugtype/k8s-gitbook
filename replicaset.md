# 레플리카셋(ReplicaSet)



* pod의 상태를 유지시켜 준다.



```
piVersion: apps/v1
kind: ReplicaSet
metadata:
  name: test-replicaset
spec:
  template:
    metadata:
      name: test-replicaset
      labels:
        app: test-replicaset
    spec:
      containers:
      - name: test-replicaset
        image: nginx
        ports:
        - containerPort: 80
  replicas: 3
  selector:
    matchLabels:
      app: test-replicaset
```









{% embed url="https://nirsa.tistory.com/136" %}
참고
{% endembed %}
