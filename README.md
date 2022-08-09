# myKubernetes
## Kubernetes

* [Prometheus&Grafana](https://github.com/Kogoon/myKubernetes/tree/main/220809)

## Minikube
`Single Node` -> Master Node + Worker Node

## Install minikube
* 설치버전: `v1.23.2`
* 작업환경: `CentOS-7`
* 요구사항: `docker`
~~~
$ yum install -y conntrack git 
~~~

* `minikube` 다운로드 
~~~
$ curl -Lo minikube https://storage.googleapis.com/minikube/releases/v1.23.2/minikube-linux-amd64 && chmod +x minikube
~~~

* `/usr/local/bin`의 디렉토리가 존재하지 않는다면 
~~~
$ mkdir -p /usr/local/bin/
~~~

* 해당 디렉토리에 `minikube` 설치 
~~~
$ install minikube /usr/local/bin/
~~~

* 설치 확인
~~~
$ minikube version
~~~


* (간펀설치)드라이버 설정x
~~~
$ minikube start --driver=none
~~~




### Kube config

~~~ bash
$ kubectl --kubeconfig=/<pathtodirectory>/my-cluster-kubeconfig.yaml get nodes
~~~

* Set&Get cluster
~~~
$ kubectl config set-cluster
$ kubectl config get-cluster
$ kubectl config get-context
~~~


