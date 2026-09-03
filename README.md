<!--lint disable awesome-contributing awesome-git-repo-age awesome-toc awesome-list-item double-link-->

# Awesome Swarm with stars

<img src="images/awesome-swarm.png" align="right" width="250" />

> An awesome list of tools and info on Swarm Mode (SwarmKit)

Swarm (Swarm Mode, SwarmKit) is the simple orchestration and scheduling system built into Moby, Docker Engine, and Mirantis Container Engine (MCE). It is a distributed system that allows you to create and manage a cluster of container runtimes (nodes) and the container workloads running on them.

This Awesome List is maintained by [@BretFisher](https://github.com/BretFisher) and [@s4ke](https://github.com/s4ke). This is a curated list of *working* and *awesome* tools and resources for using Swarm. It is not an official list, but a community effort to help people find the best stuff for Swarm in 2023 and beyond.

## Contents<!-- omit from toc -->

* [Recent News and Updates](#recent-news-and-updates)
* [Official Main Resources](#official-main-resources)
* [Chat and Forums](#chat-and-forums)
* [Community Tools](#community-tools)
  * [Cluster Management](#cluster-management)
  * [Extra Functionality](#extra-functionality)
  * [Volumes and Storage](#volumes-and-storage)
  * [Networking](#networking)
  * [Monitoring](#monitoring)
* [Community Tutorials and Education](#community-tutorials-and-education)
  * [Courses and Videos](#courses-and-videos)
  * [Articles and Sample Code](#articles-and-sample-code)
* [Organisations Using Swarm](#organisations-using-swarm)
* [RIP](#rip)
* [Contributing](#contributing)
* [Maintainers](#maintainers)

## Recent News and Updates

* 2026-03 - [Portainer - Technical Advisory: Docker Swarm](https://www.portainer.io/blog/technical-advisory-docker-swarm) - Upgrade guidance for Docker Engine API v49 compatibility changes affecting Swarm volumes, iptables, overlay networks, VXLAN, and related API clients/plugins.
* 2025-07 - [Mirantis - Mirantis guarantees long-term support for Swarm until 2030](https://www.mirantis.com/blog/mirantis-guarantees-long-term-support-for-swarm/)
* 2024-12 - [Mirantis - Introducing Mirantis Container Runtime 25](https://www.mirantis.com/blog/introducing-mirantis-container-runtime-25-enhanced-observability-extensibility-performance/)
* 2024-03 - [Mirantis - Swarm is here to stay — and will keep getting better in security and ease of operations](https://www.mirantis.com/blog/swarm-is-here-to-stay-and-keeps-getting-better-in-security-and-ease-of-operations/)
* 2023-02 - [Mirantis - Announcing the 23.0 major release for Mirantis Container Runtime — and Moby](https://www.mirantis.com/blog/announcing-the-23-0-major-release-for-mirantis-container-runtimeand-moby)
* 2022-10 - [Mirantis - What's next for Swarm](https://www.mirantis.com/blog/what-s-next-for-swarm/)
* 2022-10 - [Mirantis - Kubernetes vs Swarm - These companies use both](https://www.mirantis.com/blog/kubernetes-vs-swarm-these-companies-use-both)
* 2022-04 - [Mirantis - Committed to Swarm](https://www.mirantis.com/blog/mirantis-is-committed-to-swarm/)

## Official Main Resources

* [Docker Compose V3 File Format Docs](https://github.com/docker/compose/blob/v1/docs/Compose%20file%20reference%20\(legacy\)/version-3.md) ⭐ 38,118 | 🐛 106 | 🌐 Go | 📅 2026-09-02 - Documentation for the Docker Compose V3 format that the `docker stack` command uses.
* [SwarmKit Repository](https://github.com/moby/swarmkit) ⭐ 3,648 | 🐛 276 | 🌐 Go | 📅 2026-08-28 - The upstream project that provides Swarm features to a container runtime.
* [Docker Swarm Docs](https://docs.docker.com/engine/swarm/)
* [Mirantis Swarm Homepage](https://www.mirantis.com/software/swarm/)
* [MCR - Mirantis Container Runtime Homepage](https://www.mirantis.com/software/mirantis-container-runtime/) - The Mirantis dockerd variant that supports Swarm Mode.
* [Mirantis Docs](https://docs.mirantis.com/) - Search Swarm for the various docs related to Swarm orchestration.
* [Swarm Stack File reference](https://docs.docker.com/compose/compose-file/compose-file-v3/) - Compose file v3 format that works in Swarm for "stack files".

## Chat and Forums

* [Discord - Cloud Native DevOps](https://devops.fan) - Maintained by [Bret Fisher](https://www.bretfisher.com) and friends. Join the very active `#swarm` channel.<!--lint ignore double-link-->
* [SwarmKit.org Forum](https://swarmkit.org/forum/) - Maintained by [Portainer's](https://www.portainer.io/) co-founder Neil Cresswell.
* [Stack Overflow Swarm tag](https://stackoverflow.com/questions/tagged/docker-swarm)

## Community Tools

### Cluster Management

* [Dockersamples Swarm Visualizer](https://github.com/dockersamples/docker-swarm-visualizer) ⭐ 3,338 | 🐛 11 | 🌐 JavaScript | 📅 2024-10-26 - A basic web GUI visualizing a Swarm cluster. More of a concept and teaching UI than a production tool.
* [Swirl](https://github.com/cuigh/swirl) ⭐ 667 | 🐛 23 | 🌐 Go | 📅 2023-05-16 - Web UI for Docker, focused on swarm cluster.
* [Mohsenasm Swarm Dashboard](https://github.com/mohsenasm/swarm-dashboard) ⭐ 239 | 🐛 11 | 🌐 Elm | 📅 2026-06-05 - A Simple Monitoring Dashboard for Docker Swarm Cluster.
* [Swarmsible](https://github.com/neuroforgede/swarmsible) ⭐ 77 | 🐛 8 | 🌐 Shell | 📅 2025-02-19 - Tooling to create and manage Docker Swarm clusters based on Ansible.
* [swarmgate](https://github.com/neuroforgede/swarmgate) ⭐ 68 | 🐛 4 | 🌐 TypeScript | 📅 2025-02-19 - Multitenancy for Docker Swarm - Docker Socket Proxy for use with Docker Swarm to have multiple tenants on a single Swarm.
* [Heckenmann Swarm Dashboard](https://github.com/heckenmann/docker-swarm-dashboard) ⭐ 50 | 🐛 10 | 🌐 JavaScript | 📅 2026-09-02 - A Monitoring Dashboard for a Docker Swarm Cluster that gives you a bit more insights.
* [AWS Docker Swarm Terraform Module](https://github.com/trajano/terraform-docker-swarm-aws) ⭐ 47 | 🐛 4 | 🌐 HCL | 📅 2025-10-23
* [swarmcli](https://github.com/Eldara-Tech/swarmcli) ⭐ 21 | 🐛 17 | 🌐 Go | 📅 2026-09-02 - Swarm Management at the speed of thought — with real-time log streaming, instant shell access to containers, seamless port forwarding, and on-demand secret reveal capabilities, giving you full control over your Docker Swarm without breaking your flow.
* [MongoDB ReplicaSet Manager](https://github.com/BitWise-0x/MongoDB-ReplicaSet-Manager) ⭐ 15 | 🐛 0 | 🌐 Python | 📅 2026-04-27 - Automated deployment and management of MongoDB replica sets in Docker Swarm with intelligent failover and dynamic scaling.
* [Portainer](https://www.portainer.io/) - A management UI that allows you to control Docker hosts, Swarm clusters, and Kubernetes clusters.
* [Swarmpit](https://swarmpit.io/) - Lightweight mobile-friendly Docker Swarm management UI.
* [Spin](https://serversideup.net/open-source/spin/) - A lightweight tool that helps developers manage applications from development to production using Docker Compose, Docker Swarm, and Ansible.
* [CapRover](https://caprover.com/) - CapRover is an extremely easy to use self hosted Platform as a Service (PaaS) that uses Docker Swarm to balancer workloads across one or more servers.
* [Terraform Docker Provider](https://registry.terraform.io/providers/kreuzwerker/docker) - Infrastructure as code like stack files that supports the use of Docker services against the Docker API.

### Extra Functionality

* [doco-cd](https://github.com/kimdre/doco-cd) ⭐ 1,648 | 🐛 12 | 🌐 Go | 📅 2026-09-02 - Lightweight GitOps and Continuous Deployment tool to deploy Docker Compose projects and Swarm stacks using polling and webhooks.
* [Swarm Cronjob](https://github.com/crazy-max/swarm-cronjob) ⭐ 882 | 🐛 37 | 🌐 Go | 📅 2026-09-02 - By [@crazy-max](https://github.com/crazy-max). Create jobs on a time-based schedule.
* [Shepherd](https://github.com/djmaze/shepherd) ⭐ 594 | 🐛 13 | 🌐 Shell | 📅 2025-11-11 - Automatically update services whenever their image is refreshed.
* [SwarmCD](https://github.com/m-adawi/swarm-cd) ⭐ 188 | 🐛 41 | 🌐 Go | 📅 2026-05-20 - Declarative GitOps and Continuous Deployment tool for Swarm.
* [docker-stack-wait](https://github.com/sudo-bmitch/docker-stack-wait) ⚠️ Archived - Tool to wait for your docker stack deployments to finish.
* [Swarm Sync](https://github.com/swarm-pack/swarm-sync) ⭐ 99 | 🐛 30 | 🌐 JavaScript | 📅 2023-01-07 - GitOps for Swarm.
* [Gantry](https://github.com/shizunge/gantry) ⭐ 90 | 🐛 0 | 🌐 Shell | 📅 2026-08-25 - a tool to update docker swarm services, enhanced [Shepherd](https://github.com/djmaze/shepherd) ⭐ 594 | 🐛 13 | 🌐 Shell | 📅 2025-11-11.
* [docker-stack-deploy (docker-sdp)](https://github.com/neuroforgede/docker-stack-deploy) ⭐ 43 | 🐛 2 | 🌐 Python | 📅 2024-06-18 - Automatic config/secret rotation for Docker stacks.
* [docker-swarm-proxy](https://github.com/neuroforgede/docker-swarm-proxy) ⭐ 36 | 🐛 4 | 🌐 Python | 📅 2023-07-12 - CLI plugin to that allows to exec into services. `docker exec` for Swarm.
* [nothelm.py](https://github.com/neuroforgede/nothelm.py) ⭐ 30 | 🐛 4 | 🌐 Python | 📅 2024-07-16 - Opinionated docker stack project tool with templating support.
* [Swarm pilot](https://github.com/Integral-Systems/swarm-pilot) ⭐ 12 | 🐛 8 | 🌐 TypeScript | 📅 2026-02-11 - Scale Serices up/down by CPU & Memory Usage
* [Swarmhook](https://github.com/M4TY/swarmhook) ⭐ 9 | 🐛 0 | 🌐 TypeScript | 📅 2025-09-03 - A simple to use service that redeploys Swarm services using webhooks.

### Volumes and Storage

Swarm previously only supported local volumes, NFS, and a limited set of Docker Engine Plugin drivers that supported Swarm Mode. Driver support has dwindled over time as vendors moved to Kubernetes. In 2023, with the Docker Engine v23.x release, Docker Engine and Swarm Mode gained the Container Storage Interface (CSI) standard. Existing CSI drivers will need to add Swarm support.

* [juicefs](https://github.com/juicedata/juicefs) ⭐ 14,387 | 🐛 200 | 🌐 Go | 📅 2026-09-02 - JuiceFS is a distributed POSIX file system built on top of S3. It has a maintained [Docker plugin](https://github.com/juicedata/docker-volume-juicefs) ⭐ 45 | 🐛 14 | 🌐 Go | 📅 2026-08-17.
* [Ceph](https://ceph.io/) - Ceph is a distributed object, block, and file storage platform. **Do you want Ceph CSI support? [Upvote this issue](https://github.com/ceph/ceph-csi/issues/3769) ⭐ 1,572 | 🐛 153 | 🌐 Go | 📅 2026-09-02**
* [NetApp Trident](https://github.com/NetApp/trident) ⭐ 876 | 🐛 276 | 🌐 Go | 📅 2026-08-27 - A NetApp storage driver that has been known to work with Docker Engine and Swarm in the past. CSI Swarm support [has been requested](https://github.com/NetApp/trident/issues/804) ⭐ 876 | 🐛 276 | 🌐 Go | 📅 2026-08-27.
* [Hetzner Cloud Volume CSI Driver](https://github.com/hetznercloud/csi-driver) ⭐ 795 | 🐛 24 | 🌐 Go | 📅 2026-09-02 - Hetzner Cloud Volume CSI Driver with experimental support for Docker Swarm.
* [Hetzner Cloud Docker Volume Plugin](https://github.com/costela/docker-volume-hetzner) ⭐ 119 | 🐛 8 | 🌐 Go | 📅 2026-08-31 - Unofficial volume driver for [Hetzner Cloud](https://www.hetzner.com/cloud) by [@costela](https://github.com/costela).
* [Docker Volume plugin for RBD (Ceph)](https://github.com/wetopi/docker-volume-rbd) ⭐ 95 | 🐛 9 | 🌐 Go | 📅 2024-02-28 - Docker Engine managed plugin to for RBD Ceph volumes.
* [CSI support issue tracking in 2023](https://github.com/olljanat/csi-plugins-for-docker-swarm) ⭐ 81 | 🐛 11 | 🌐 Shell | 📅 2025-04-01 - A GitHub repository tracking various storage drivers PRs and issues for Swarm CSI support in Docker/Moby v23+.
* [GlusterFS](https://www.gluster.org/) - GlusterFS is a scale-out network-attached storage file system.
* [Portworx](https://docs.portworx.com/install-portworx/install-with-other/docker/swarm/) - Portworx is a container-native storage solution. It [supports Swarm installs](https://docs.portworx.com/install-portworx/install-with-other/docker/swarm/). Free for up to three nodes.

### Networking

* [Traefik Proxy](https://github.com/traefik/traefik) ⭐ 64,713 | 🐛 911 | 🌐 Go | 📅 2026-09-02 - A reverse proxy and load balancer that makes deploying HTTP (and more) published services easy. Swarm Mode docs [start here](https://doc.traefik.io/traefik/providers/docker/#docker-swarm-mode).
* [Caddy Docker Proxy](https://github.com/lucaslorentz/caddy-docker-proxy) ⭐ 4,637 | 🐛 49 | 🌐 Go | 📅 2026-08-20 - Caddy based reverse proxy with automatic service discovery based on labels.
* [Libnetwork Troubleshooting](https://github.com/moby/libnetwork/blob/master/cmd/diagnostic/README.md) ⭐ 2,207 | 🐛 207 | 🌐 Go | 📅 2023-10-20 - Official Doc on using network diagnostic tools.
* [rawdns](https://github.com/tianon/rawdns) ⭐ 214 | 🐛 8 | 🌐 Go | 📅 2026-06-06 - a direct, raw DNS interface to the Docker API.
* [envoy-swarm-control-plane](https://github.com/nstapelbroek/envoy-swarm-control-plane) ⭐ 39 | 🐛 6 | 🌐 Go | 📅 2026-09-02 - Software that helps Envoy route internet traffic towards your microservices running on Docker Swarm.
* [Swarm Ports](https://www.bretfisher.com/docker-swarm-firewall-ports/) - List and description of all the ports used by Swarm Mode (and the very old classic Swarm, if you're into that).

### Monitoring

* [promswarm](https://github.com/neuroforgede/promswarm) ⭐ 32 | 🐛 1 | 🌐 Jinja | 📅 2024-04-06 - Modernized version of [Swarmprom](https://github.com/stefanprodan/swarmprom) ⚠️ Archived, a great Prometheus/Grafana stack originally by [@stefanprodan](https://github.com/stefanprodan), now maintained by [@neuroforgede](https://github.com/neuroforgede).
* [docker-engine-events-exporter](https://github.com/neuroforgede/docker-engine-events-exporter) ⭐ 18 | 🐛 3 | 🌐 Python | 📅 2026-06-20 - Prometheus Exporter for Docker Engine Events.
* [docker-engine-networks-exporter](https://github.com/neuroforgede/docker-engine-networks-exporter) ⭐ 10 | 🐛 0 | 🌐 Python | 📅 2026-05-17 - Prometheus Exporter for additional network metrics such as usable ips.

## Community Tutorials and Education

### Courses and Videos

* [Docker Mastery, with Kubernetes and Swarm](https://bret.show/dockermastery) - Via Docker Captain Bret Fisher. The most popular paid mega-course on Docker, Kubernetes, and Swarm. The link includes a coupon.
* [Docker Swarm Mastery](https://bret.show/swarmmastery) - Via Docker Captain Bret Fisher. The most popular paid course focusing on Docker Swarm (assumes you have basic Docker/Compose knowledge). The link includes a coupon.
* [Docker Swarm Design and Production Tools from Bret Fisher at DockerCon](https://www.youtube.com/watch?v=V9fxU5zJKb4) - YouTube. DockerCon 2018. 40 minutes.

### Articles and Sample Code

* [dogvs.cat Sample Swarm Stacks](https://github.com/BretFisher/dogvscat) ⭐ 525 | 🐛 10 | 🌐 HCL | 📅 2023-01-07 - Sample Docker Swarm cluster stack of tools including Traefik.
* [Swarm vs. Compose for Production](https://github.com/BretFisher/ama/discussions/146) ⭐ 362 | 🐛 0 | 📅 2021-08-23 - Only one host for a production environment. What to use: docker-compose or single node swarm?
* [Podlike](https://github.com/rycus86/podlike) ⭐ 87 | 🐛 8 | 🌐 Go | 📅 2023-05-11 - Viktor Adam's idea on how you could link multiple containers together to emulate a Kubernetes pod.
* [Docker Swarm Rocks](https://dockerswarm.rocks/) - Collection of tutorials and code samples.
* [Docker Swarm Still Rocks](https://dockerswarmstill.rocks/) - Continuation of above site with updated tutorials and code samples.
* [Vault + Swarm](https://blog.sunekeller.dk/2019/04/vault-swarm-plugin-poc/) - Vault + Swarm Docker secrets plugin (proof of concept).
* [Cheat Sheet on Docker and Swarm 2022](https://cheatography.com/boulard/cheat-sheets/docker-and-swarm-2022/)
* [Operating Swarm](https://containers.goffinet.org/swarm/operatingswarm.html) - Useful tips for operating and troubleshooting Docker Swarm in production.

## Organisations Using Swarm

* [Co-op Cloud](https://coopcloud.tech)
* [NeuroForge](https://neuroforge.de)

## Related Awesome Lists

While this list is focused on Docker Swarm resources, general resources such as ones for Docker or Docker Compose can be helpful. The following keeps track of related awesome lists focused on this.

* [awesome-compose](https://github.com/docker/awesome-compose) ⭐ 46,218 | 🐛 418 | 🌐 HTML | 📅 2026-09-01 - A list of awesome Docker Compose samples.
* [awesome-docker](https://github.com/veggiemonk/awesome-docker) ⭐ 36,764 | 🐛 27 | 📅 2026-08-27 - A list of awesome Docker tools.

## RIP

Honorable mentions of tools and information that are no longer maintained or supported. It may still work, but it's not being updated.

* [RexRay](https://github.com/rexray/rexray) ⭐ 2,222 | 🐛 294 | 🌐 Go | 📅 2023-09-02 - A container storage orchestration engine.

## Contributing

This list thrives on contributions from the community. The Maintainers can't do it alone. We need Swarm fans to help us find the best Swarm resources.

Want to contribute? Please read the [contribution guidelines](contributing.md). You can also ask questions in the [GitHub Discussions](https://github.com/BretFisher/awesome-swarm/discussions) ⭐ 747 | 🐛 7 | 📅 2026-08-19, or our [Discord Server #swarm channel](https://discord.gg/4jPPynEb2e).

## Maintainers

We're looking for more maintainers. Make some PRs to help, then LMK in Discussions, Twitter, or Discord (above) if you'd like to get involved in making a better community for Swarm.

***

> _Enhansomed by [enhansome](https://github.com/enhansome) on 2026-09-03._
