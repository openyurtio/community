# Roadmap

This document outlines the development roadmap for the OpenYurt project. And the details of roadmap before 2023 is
managed in `openyurtio/openyurt` repo, the link is here: https://github.com/openyurtio/openyurt/blob/master/docs/roadmap.md

## 2023 Roadmap

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

- openyurtio/yurt-dashboard repo

    - support logs/exec pods on edge nodes from console
    - support raven
    - support pool-coordinator
    - hope to have more than 100+ users to try OpenYurt experience center

**SIG DataPlane**


**SIG IoT**
