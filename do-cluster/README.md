# Digital Ocean

### doctl

* available regions 

~~~ bash
$ doctl kubernetes options regions
~~~


* Available kubernetes versions

~~~ bash
$ doctl kubernetes options versions
~~~


* Available node's size

~~~ bash
$ doctl kubernetes options sizes
~~~

### Cluster

* Create a cluster with 3 nodes

~~~ bash
$ doctl k c create my-cluster --version 1.22.11-do.0 --region sfo3 --node-pool "name=workers;size=s-1vcpu-2gb;count=3;"
~~~
   * kubernetes version `1.22.11`
   * region `sfo3` - San Francisco region
   * node-pool - node info 
      * name  - workers
      * size  - (basic)s-1vcpu-2gb
      * count - 3
