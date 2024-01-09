# Roadmap

**SIG ControlPlane**

- openyurtio/openyurt repo:

  - yurt-manager
    - move scattered controllers into yurt-controller-manager ([#1067](https://github.com/openyurtio/openyurt/issues/1067))
    - support OTA and Auto upgrade model for static pod ([#1079](https://github.com/openyurtio/openyurt/issues/1079))
    - YurtAppDaemon: support each nodePool can be configured independently

  - yurthub
    - install yurthub component on edge nodes depending on StaticPod cr resource ([#1080](https://github.com/openyurtio/openyurt/issues/1080))
    - support filter chain to mutate response data in YurtHub [#1188](https://github.com/openyurtio/openyurt/issues/1188)
    - support NodePort service isolated for specified nodePool [#1183](https://github.com/openyurtio/openyurt/issues/1183)

  - pool-coordinator:
    - support monitor or logs/exec nodePool resource when cloud-edge network off
    - support share traffic in NodePool between cloud and edge for CRD resource
    - support seamlessly break traffic to crashed instance when cloud-edge network off
    - improve metrics/events/logs

  - yurtadm
    - support yurtadm init command based on sealer

  - e2e
    - combine yurtctl tool into e2e tool ([#1059](https://github.com/openyurtio/openyurt/issues/1059))
    - support pool-coordinator
    - support raven and remove yurt-tunnel

  - beehive
    - a new component for providing tenant isolation management, end user can join nodes can deploy workloads, but they can access or view their own resources.
    - the new component will be hosted in openyurt repo.

**SIG DataPlane**

- support SLB as public network exporter for gateway ([#22](https://github.com/openyurtio/raven/issues/22))
- add reconciliation loop to check route entries and vpn connections periodically. ([#10](https://github.com/openyurtio/raven/issues/10))
- [Raven-L7] Endpoints manager implementation ([#69](https://github.com/openyurtio/raven/issues/69))
- [Raven-L7] Raven l7 proxy implementation ([#70](https://github.com/openyurtio/raven/issues/70))
- [Raven-L7] DNS manager implementation ([#66](https://github.com/openyurtio/raven/issues/66))
- [Raven-L7] Cert manager implementation ([#67](https://github.com/openyurtio/raven/issues/67))
- support to use helm to deploy raven ([#73](https://github.com/openyurtio/raven/issues/73))

**SIG IoT**

- release EdgeX-Auto-Collector to help support later EdgeX versions automatically ([#24](https://github.com/openyurtio/yurt-edgex-manager/issues/24))
- add security component for EdgeX ([#13](https://github.com/openyurtio/yurt-edgex-manager/issues/13))
- refactor yurt-edgex-manager to yurt-iot-manager ([#92](https://github.com/openyurtio/yurt-edgex-manager/issues/92))
- provide a video analytical reference architecture and implementation based on OpenYurt + EdgeX + OpenVINO ([#33](https://github.com/openyurtio/yurt-device-controller/issues/33)) 
- support other IoT platforms similar to EdgeX ([#93](https://github.com/openyurtio/yurt-edgex-manager/issues/93))
- Yurt IoT Dataflow: provide dataflow orchestration framework to help better process IoT device data

**SIG UI/CLI**

- automated installation and deployment platform based on dashboard ([#41](https://github.com/openyurtio/yurt-dashboard/issues/41)])
- upgrade dashboard API to latest OpenYurt version ([#43](https://github.com/openyurtio/yurt-dashboard/issues/43))
- support join node in specific nodepool ([#1380](https://github.com/openyurtio/openyurt/issues/1380))
- provide --config option for yurtadm ([#1448](https://github.com/openyurtio/openyurt/issues/1448))
