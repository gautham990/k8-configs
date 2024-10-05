### Cluster Autoscaler in EKS
* Reference doc: https://www.stacksimplify.com/aws-eks/aws-eks-kubernetes-autoscaling/learn-to-master-cluster-autoscaler-on-aws-eks/
* Change the CA image version to match the EKS cluter version. Also note that image registry has been changed. CA releases with image version can be found at https://github.com/kubernetes/autoscaler/releases
* Modify the `--node-group-auto-discovery=` to match the tags of ASG. In the test runit was set to `k8s.io/cluster-autoscaler/enabled=true` and `k8s.io/cluster-autoscaler/<CLUSTER_NAME>=owned`
