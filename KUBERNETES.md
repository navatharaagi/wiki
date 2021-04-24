# K8s 

### K8S Architecture 

[K8S Components](https://kubernetes.io/docs/concepts/overview/components/)
* Master (Control Plane) (Multiple Maters)
  * 4 Process on every master node 
    * API Server (Cluster Gateway)
      * Gatekeeper for authentication 
    * Scheduler
    * Controller Manager 
      * Detect Cluster state changes 
    * etcd 
      * Key value store of cluster state (brain...!)
* Node (Worker Machine)
  * Each node has multiple pods 
  * 3 Process must be installed on all nodes 
    * Kubelet (Intreacts with container and node )
    * Kube Proxy (Forwarding requests)
    * Container Runtime 

### K8S Basic Objects  
 * Node (Physical or Virtual Server)
 * Pod 
   * Smallest unit of K8s 
   * Abstraction over container 
   * Usually 1 application per pod 
   * Each pod gets its own IP address 
   * New IP address on re-creation 
 * Service 
   * Permanent IP address 
   * Lifecycle of pod and service are not connected 
   * Loadbalancer 
 * Ingress 
   * Route traffic into cluster 
 * ConfigMap
   * Configuration of application (Properties)
 * Secret
   * Used to store secret data (base64 encoded) 
 * Volumes 
   * Attach Physical storage 
     * Local 
     * Remote (Cloud / External storage)
 * Deployments 
   * Blueprint for pods (apps)
   * Stateless apps 
 * Statefulset 
   * Stateful apps 


 


    
