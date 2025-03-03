Manifest 1 Values:
cilium_helm_parameters:
  - name: ipam.mode
    value: kubernetes
  - name: kubeProxyReplacement
    value: "true"
  - name: securityContext.capabilities.ciliumAgent
    value: "{CHOWN,KILL,NET_ADMIN,NET_RAW,IPC_LOCK,SYS_ADMIN,SYS_RESOURCE,DAC_OVERRIDE,FOWNER,SETGID,SETUID}"
  - name: securityContext.capabilities.cleanCiliumState
    value: "{NET_ADMIN,SYS_ADMIN,SYS_RESOURCE}"
  - name: cgroup.autoMount.enabled
    value: "false"
  - name: cgroup.hostRoot
    value: /sys/fs/cgroup
  - name: k8sServiceHost
    value: localhost
  - name: k8sServicePort
    value: "7445"
  - name: ipv6.enabled
    value: "false"
  - name: securityContext.privileged
    value: "true"
  - name: envoy.enabled
    value: "true"


Manifest 2 Values:
cilium_helm_parameters:
  - name: ipam.mode
    value: kubernetes
  - name: kubeProxyReplacement
    value: "true"
  - name: securityContext.capabilities.ciliumAgent
    value: "{CHOWN,KILL,NET_ADMIN,NET_RAW,IPC_LOCK,SYS_ADMIN,SYS_RESOURCE,DAC_OVERRIDE,FOWNER,SETGID,SETUID}"
  - name: securityContext.capabilities.cleanCiliumState
    value: "{NET_ADMIN,SYS_ADMIN,SYS_RESOURCE}"
  - name: cgroup.autoMount.enabled
    value: "false"
  - name: cgroup.hostRoot
    value: /sys/fs/cgroup
  - name: k8sServiceHost
    value: localhost
  - name: k8sServicePort
    value: "7445"
  - name: ipv6.enabled
    value: "false"
  - name: securityContext.privileged
    value: "true"
  - name: envoy.enabled
    value: "true"
  - name: ingressController.enabled
    value: "true"
  - name: ingressController.controller.service.enabled
    value: "true"
  - name: ingressController.loadbalancerMode
    value: "dedicated"
  - name: l7Proxy
    value: "true"
  - name: nodePort.enabled
    value: "true"
  - name: global.crds.install
    value: "true"
