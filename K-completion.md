## Kubectl Completion and Alias

* kubectl command 자동 완성 

~~~ bash
# echo 'source <(kubectl completion bash)' >>~/.bashrc
~~~


* Alias kubectl

~~~ bash
$ echo 'alias k=kubectl' >>~/.bashrc
~~~


* 별칭 k 의 자동완성 

~~~ bash
$ echo 'complete -F __start_kubectl k' >>~/.bashrc
~~~


