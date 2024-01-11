# Roadmap

**SIG ControlPlane**

  - support LoadBalancer Service in multiple nodepools
    - support Load Balancer (LB) across multiple NodePools, ensuring high availability and fault tolerance for edge applications by seamlessly redirecting traffic during node disruptions.
    - a new component will be resided on edge nodes as daemon pod.

  - support Ingress Controller in multiple nodepools
    - advanced Ingress Controller supports multiple NodePools, optimizing application traffic distribution and security across OpenYurt cluster for a streamlined edge computing experience.
    - each nodepool deploys a separate set of Nginx controllers..

  - yurt-express
    - a new component offers seamless bidirectional communication between cloud and edge, enabling effortless data and file transfers via HTTP(s) and MQTT. It's designed to handle logs and AI model files seamlessly, requiring no code modifications. This robust solution is perfect for end-users in areas with weak network connectivity.
    - the new component will be hosted in openyurt repo.

  - beehive
    - a new component for providing namespace tenant isolation management, end users can join nodes and deploy workloads, but they can access or view their own resources.
    - the new component will be hosted in openyurt repo.

  - scalability
    - Supporting a large number of edge nodes and providing lightweight runtime solutions is a high demand for edge computing. Kubernetes has its own limitations in terms of the supported number of nodes and the resource overhead for node daemons. Instead of providing a one-for-all approach, we have decided to propose a different architecture to handle cases where the cluster scale can exceed the supported number. We have found that once the cluster scale reaches a certain limit, the design tradeoffs and considerations become very different in edge use cases. We have planned to form a new SIG for scalability which will be focusing on exploring techniques to make supporting millions of edge nodes in a single cloud apiserver possible (an ambitious goal) and reduce the node daemon overhead to a minimum level.

**SIG DataPlane**

- add reconciliation loop to check route entries and vpn connections periodically. ([#10](https://github.com/openyurtio/raven/issues/10))
- Path selection policy after Layer 3 NAT traversal is supported ([#143](https://github.com/openyurtio/raven/issues/143))
- Develop a new seven-layer network proxy package to replace anp and remove the interceptor module to reduce the number of proxy hops ([#142](https://github.com/openyurtio/raven/issues/142))
- Integrate raven into the openyurt repository ([#145](https://github.com/openyurtio/raven/issues/145))
- Optimized the centre gateway election policy ([#146](https://github.com/openyurtio/raven/issues/146))
- The observability of raven's cross-edge traffic ([#144](https://github.com/openyurtio/raven/issues/144))

**SIG IoT**


**SIG UI/CLI**

