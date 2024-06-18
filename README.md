# CKS-Tips : Certified kubernetes security specialist

For the CK exam here are the points and concepts to focus on:
- create a serviceaccount without installing the default tokens
- create a pod and set up a serviceaccount
- create a runtimeClass: runsc or gvisor
- create a pod with the runtimeClass create
- define cipherSuite at the cluster level (api-server and etcd) TLS_ECDHE_ECDSA_WITH_AES_128_GCM_SHA256, tlsversion:1.2
- Create network policies to block all traffic entering a namespace testing
- Create network policies to block all traffic leaving a namespace
- activated auditing within the cluster (adapt the policy.yaml provided)
- CIS Benchmarck with Kube-bench
- used falco to detect abnormal behavior generating in a pod
- Configure the ingress in HTTPS: you must create the TLS secret and mount it in the ingress
- used trivy to scan images and remove images that are more vulnerable
- you are given a Dockerfile and a Kubernetes manifest: make two modifications in each of the files to correct the bad practices that you will detect
- activated the imagepolicyWebhook plugin and import admission-controler-config-file which will be provided: create the pod and check
- we give an apparmor profile, use it to reinforce the security of the pod at the level of the Node on which it is deployed
- immutable
- RBAC: create role, rolebinding, clusterrole, clusterrolebinding
- delete the user: system:anonymous
