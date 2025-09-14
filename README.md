# k8s-scheduling
Repository for practicing Kubernetes scheduling concepts such as node selectors, affinity, anti-affinity, taints, and tolerations. Includes real-world use cases like Redis and Web Server deployments for high availability and performance optimization.

This repository contains hands-on practice with Kubernetes scheduling concepts such as **node selectors, node affinity, node anti-affinity, pod affinity, pod anti-affinity, taints, and tolerations**.  
It demonstrates how scheduling rules impact pod placement, isolation, high availability, and performance in real-world scenarios.


# EBS - install drivers
-------------------
kubectl apply -k "github.com/kubernetes-sigs/aws-ebs-csi-driver/deploy/kubernetes/overlays/stable/?ref=release-1.43"

# EFS - install drivers
------------------------
kubectl kustomize \
    "github.com/kubernetes-sigs/aws-efs-csi-driver/deploy/kubernetes/overlays/stable/ecr/?ref=release-2.1" > private-ecr-driver.yaml