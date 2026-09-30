# DevOps Interview World

Practical DevOps, SRE, and Platform Engineering interview preparation by VERIQTA.

Practice diagnosing failed services, troubleshooting containers, repairing delivery pipelines, investigating cloud connectivity, and following requests through metrics, logs, and traces. Explain your decisions with evidence, then show how you verify recovery.

![DevOps Interview World by VERIQTA](assets/cover.svg)

## 150 practical interview questions

Explore 25 tool areas, with 50 Junior, 50 Mid-Level, and 50 Senior questions. Each title opens its interview question file.

**Current edition:** All 150 question briefs are included. Runnable labs, step-by-step solutions, and video walkthroughs are not included yet. This is the question catalogue edition.

If this repository helps your preparation, star it and share it with another engineer.

## Browse by tool

| Area | Tools and subjects | Questions |
|---|---|---|
| [Linux](#linux) | Linux, systemd | 6 |
| [Bash](#bash) | Bash, core utilities | 6 |
| [Git](#git) | Git, GitHub | 6 |
| [Networking](#networking) | DNS, TCP/IP, HTTP, TLS, Nginx | 6 |
| [Docker](#docker) | Docker, Docker Compose | 6 |
| [Builds and registries](#builds-and-registries) | BuildKit, Buildx, Docker Hub, ECR, ACR, Artifact Registry | 6 |
| [Podman and runtimes](#podman-and-runtimes) | Podman, containerd, CRI-O | 6 |
| [Kubernetes workloads](#kubernetes-workloads) | Kubernetes, kubectl | 6 |
| [Kubernetes platform](#kubernetes-platform) | Kubernetes, RBAC, Services, storage | 6 |
| [Helm and Kustomize](#helm-and-kustomize) | Helm, Kustomize | 6 |
| [AWS foundations](#aws-foundations) | AWS IAM, VPC, EC2, S3, Route 53 | 6 |
| [AWS applications](#aws-applications) | AWS ALB, Lambda, API Gateway, DynamoDB, EKS | 6 |
| [Azure](#azure) | Azure networking, VMs, AKS, ACR, managed identity | 6 |
| [Google Cloud](#google-cloud) | Compute Engine, IAM, GKE, Cloud Run, Artifact Registry | 6 |
| [Terraform](#terraform) | Terraform | 6 |
| [Ansible](#ansible) | Ansible | 6 |
| [Jenkins](#jenkins) | Jenkins, agents, credentials | 6 |
| [GitHub Actions](#github-actions) | GitHub Actions, artifacts, environments | 6 |
| [GitLab and Azure pipelines](#gitlab-and-azure-pipelines) | GitLab CI/CD, Azure Pipelines | 6 |
| [GitOps](#gitops) | Argo CD, Flux, Git, Kubernetes | 6 |
| [Metrics](#metrics) | Prometheus, Grafana, PromQL | 6 |
| [Logs](#logs) | Fluent Bit, Fluentd, Loki, Elasticsearch, Logstash, Kibana | 6 |
| [Tracing and alerting](#tracing-and-alerting) | OpenTelemetry, Jaeger, Tempo, Alertmanager, Grafana Alerting | 6 |
| [Cloud and commercial telemetry](#cloud-and-commercial-telemetry) | CloudWatch, Azure Monitor, Google Cloud Monitoring and Logging, Datadog, New Relic | 6 |
| [Security automation and combined incidents](#security-automation-and-combined-incidents) | Trivy, Python, Linux, Kubernetes, CI/CD, observability | 6 |

## Choose your level

| Level | What the interview tests |
|---|---|
| Junior | Bounded tasks, correct commands, and basic verification |
| Mid-Level | Investigation across components, root cause, and controlled recovery |
| Senior | Ambiguous incidents, tradeoffs, risk, and prevention |

## All 150 questions

### Linux

| # | Interview question | Difficulty |
|---|---|---|
| 001 | [Diagnose a service that fails after restart](linux/DIW-001-diagnose-a-service-that-fails-after-restart.md) | Junior |
| 002 | [Find the largest consumers of disk space](linux/DIW-002-find-the-largest-consumers-of-disk-space.md) | Junior |
| 003 | [Recover space held by deleted open files](linux/DIW-003-recover-space-held-by-deleted-open-files.md) | Mid-Level |
| 004 | [Investigate memory pressure without an OOM event](linux/DIW-004-investigate-memory-pressure-without-an-oom-event.md) | Mid-Level |
| 005 | [Diagnose high load with low CPU usage](linux/DIW-005-diagnose-high-load-with-low-cpu-usage.md) | Senior |
| 006 | [Recover a service affected by file descriptor exhaustion](linux/DIW-006-recover-a-service-affected-by-file-descriptor-exhaustion.md) | Senior |

### Bash

| # | Interview question | Difficulty |
|---|---|---|
| 007 | [Handle command failures and exit codes](bash/DIW-007-handle-command-failures-and-exit-codes.md) | Junior |
| 008 | [Validate script arguments and input](bash/DIW-008-validate-script-arguments-and-input.md) | Junior |
| 009 | [Preserve failure status across pipelines](bash/DIW-009-preserve-failure-status-across-pipelines.md) | Mid-Level |
| 010 | [Prevent overlapping scheduled script runs](bash/DIW-010-prevent-overlapping-scheduled-script-runs.md) | Mid-Level |
| 011 | [Make a deployment script recover from partial failure](bash/DIW-011-make-a-deployment-script-recover-from-partial-failure.md) | Senior |
| 012 | [Design reliable backup validation and retention](bash/DIW-012-design-reliable-backup-validation-and-retention.md) | Senior |

### Git

| # | Interview question | Difficulty |
|---|---|---|
| 013 | [Recover a commit after reset](git/DIW-013-recover-a-commit-after-reset.md) | Junior |
| 014 | [Resolve and verify a merge conflict](git/DIW-014-resolve-and-verify-a-merge-conflict.md) | Junior |
| 015 | [Apply a hotfix while preserving unfinished work](git/DIW-015-apply-a-hotfix-while-preserving-unfinished-work.md) | Mid-Level |
| 016 | [Recover from an incorrect rebase](git/DIW-016-recover-from-an-incorrect-rebase.md) | Mid-Level |
| 017 | [Remove an exposed secret and complete remediation](git/DIW-017-remove-an-exposed-secret-and-complete-remediation.md) | Senior |
| 018 | [Recover a release after an incorrect history rewrite](git/DIW-018-recover-a-release-after-an-incorrect-history-rewrite.md) | Senior |

### Networking

| # | Interview question | Difficulty |
|---|---|---|
| 019 | [Diagnose hostname failure when IP access works](networking/DIW-019-diagnose-hostname-failure-when-ip-access-works.md) | Junior |
| 020 | [Identify the process listening on a port](networking/DIW-020-identify-the-process-listening-on-a-port.md) | Junior |
| 021 | [Trace a connection blocked by routing or firewall rules](networking/DIW-021-trace-a-connection-blocked-by-routing-or-firewall-rules.md) | Mid-Level |
| 022 | [Diagnose TLS certificate chain failures](networking/DIW-022-diagnose-tls-certificate-chain-failures.md) | Mid-Level |
| 023 | [Investigate intermittent reverse proxy 502 responses](networking/DIW-023-investigate-intermittent-reverse-proxy-502-responses.md) | Senior |
| 024 | [Diagnose packet loss across application dependencies](networking/DIW-024-diagnose-packet-loss-across-application-dependencies.md) | Senior |

### Docker

| # | Interview question | Difficulty |
|---|---|---|
| 025 | [Diagnose a container that exits immediately](containers/docker/DIW-025-diagnose-a-container-that-exits-immediately.md) | Junior |
| 026 | [Fix container access to a mounted file](containers/docker/DIW-026-fix-container-access-to-a-mounted-file.md) | Junior |
| 027 | [Restore communication between Compose services](containers/docker/DIW-027-restore-communication-between-compose-services.md) | Mid-Level |
| 028 | [Diagnose container memory termination](containers/docker/DIW-028-diagnose-container-memory-termination.md) | Mid-Level |
| 029 | [Recover an application with incorrect signal handling](containers/docker/DIW-029-recover-an-application-with-incorrect-signal-handling.md) | Senior |
| 030 | [Investigate CPU throttling and application latency](containers/docker/DIW-030-investigate-cpu-throttling-and-application-latency.md) | Senior |

### Builds and registries

| # | Interview question | Difficulty |
|---|---|---|
| 031 | [Fix an incorrect Docker build context](containers/builds-and-registries/DIW-031-fix-an-incorrect-docker-build-context.md) | Junior |
| 032 | [Tag and verify an image by commit SHA](containers/builds-and-registries/DIW-032-tag-and-verify-an-image-by-commit-sha.md) | Junior |
| 033 | [Build and test AMD64 and ARM64 images](containers/builds-and-registries/DIW-033-build-and-test-amd64-and-arm64-images.md) | Mid-Level |
| 034 | [Diagnose registry push and pull authentication](containers/builds-and-registries/DIW-034-diagnose-registry-push-and-pull-authentication.md) | Mid-Level |
| 035 | [Trace stale image deployment despite a successful build](containers/builds-and-registries/DIW-035-trace-stale-image-deployment-despite-a-successful-build.md) | Senior |
| 036 | [Secure build credentials and verify they are absent from image layers](containers/builds-and-registries/DIW-036-secure-build-credentials-and-verify-they-are-absent-from-image-layers.md) | Senior |

### Podman and runtimes

| # | Interview question | Difficulty |
|---|---|---|
| 037 | [Run and inspect a rootless Podman container](containers/runtimes/DIW-037-run-and-inspect-a-rootless-podman-container.md) | Junior |
| 038 | [Diagnose rootless bind mount ownership](containers/runtimes/DIW-038-diagnose-rootless-bind-mount-ownership.md) | Junior |
| 039 | [Repair Podman container network connectivity](containers/runtimes/DIW-039-repair-podman-container-network-connectivity.md) | Mid-Level |
| 040 | [Investigate runtime image and container state with crictl](containers/runtimes/DIW-040-investigate-runtime-image-and-container-state-with-crictl.md) | Mid-Level |
| 041 | [Diagnose a node runtime failure using containerd evidence](containers/runtimes/DIW-041-diagnose-a-node-runtime-failure-using-containerd-evidence.md) | Senior |
| 042 | [Diagnose a node runtime failure using CRI-O evidence](containers/runtimes/DIW-042-diagnose-a-node-runtime-failure-using-cri-o-evidence.md) | Senior |

### Kubernetes workloads

| # | Interview question | Difficulty |
|---|---|---|
| 043 | [Diagnose CrashLoopBackOff](kubernetes/workloads/DIW-043-diagnose-crashloopbackoff.md) | Junior |
| 044 | [Fix a Pod with invalid configuration](kubernetes/workloads/DIW-044-fix-a-pod-with-invalid-configuration.md) | Junior |
| 045 | [Investigate ImagePullBackOff](kubernetes/workloads/DIW-045-investigate-imagepullbackoff.md) | Mid-Level |
| 046 | [Diagnose an unschedulable Pod](kubernetes/workloads/DIW-046-diagnose-an-unschedulable-pod.md) | Mid-Level |
| 047 | [Recover a rollout blocked by readiness failures](kubernetes/workloads/DIW-047-recover-a-rollout-blocked-by-readiness-failures.md) | Senior |
| 048 | [Investigate intermittent OOM kills during traffic spikes](kubernetes/workloads/DIW-048-investigate-intermittent-oom-kills-during-traffic-spikes.md) | Senior |

### Kubernetes platform

| # | Interview question | Difficulty |
|---|---|---|
| 049 | [Find why a Service has no endpoints](kubernetes/platform/DIW-049-find-why-a-service-has-no-endpoints.md) | Junior |
| 050 | [Grant read-only namespace access](kubernetes/platform/DIW-050-grant-read-only-namespace-access.md) | Junior |
| 051 | [Diagnose a PersistentVolumeClaim that remains Pending](kubernetes/platform/DIW-051-diagnose-a-persistentvolumeclaim-that-remains-pending.md) | Mid-Level |
| 052 | [Restore cluster DNS resolution](kubernetes/platform/DIW-052-restore-cluster-dns-resolution.md) | Mid-Level |
| 053 | [Investigate ingress failure across network boundaries](kubernetes/platform/DIW-053-investigate-ingress-failure-across-network-boundaries.md) | Senior |
| 054 | [Diagnose node pressure and workload eviction](kubernetes/platform/DIW-054-diagnose-node-pressure-and-workload-eviction.md) | Senior |

### Helm and Kustomize

| # | Interview question | Difficulty |
|---|---|---|
| 055 | [Render and inspect a Helm chart](kubernetes/configuration/DIW-055-render-and-inspect-a-helm-chart.md) | Junior |
| 056 | [Build and compare Kustomize overlays](kubernetes/configuration/DIW-056-build-and-compare-kustomize-overlays.md) | Junior |
| 057 | [Fix incorrect Helm values precedence](kubernetes/configuration/DIW-057-fix-incorrect-helm-values-precedence.md) | Mid-Level |
| 058 | [Repair a Kustomize patch that targets the wrong resource](kubernetes/configuration/DIW-058-repair-a-kustomize-patch-that-targets-the-wrong-resource.md) | Mid-Level |
| 059 | [Recover a failed Helm upgrade with persistent data constraints](kubernetes/configuration/DIW-059-recover-a-failed-helm-upgrade-with-persistent-data-constraints.md) | Senior |
| 060 | [Investigate configuration drift across release environments](kubernetes/configuration/DIW-060-investigate-configuration-drift-across-release-environments.md) | Senior |

### AWS foundations

| # | Interview question | Difficulty |
|---|---|---|
| 061 | [Diagnose S3 access denied for a workload](cloud/aws/foundations/DIW-061-diagnose-s3-access-denied-for-a-workload.md) | Junior |
| 062 | [Verify DNS records in a Route 53 hosted zone](cloud/aws/foundations/DIW-062-verify-dns-records-in-a-route-53-hosted-zone.md) | Junior |
| 063 | [Restore private subnet outbound access through NAT](cloud/aws/foundations/DIW-063-restore-private-subnet-outbound-access-through-nat.md) | Mid-Level |
| 064 | [Diagnose an EC2 instance unreachable through its intended access path](cloud/aws/foundations/DIW-064-diagnose-an-ec2-instance-unreachable-through-its-intended-access-path.md) | Mid-Level |
| 065 | [Investigate conflicting IAM policy decisions](cloud/aws/foundations/DIW-065-investigate-conflicting-iam-policy-decisions.md) | Senior |
| 066 | [Design least-privilege access and verify allowed and denied operations](cloud/aws/foundations/DIW-066-design-least-privilege-access-and-verify-allowed-and-denied-operations.md) | Senior |

### AWS applications

| # | Interview question | Difficulty |
|---|---|---|
| 067 | [Deploy and invoke a Lambda function](cloud/aws/applications/DIW-067-deploy-and-invoke-a-lambda-function.md) | Junior |
| 068 | [Investigate an API Gateway request failure](cloud/aws/applications/DIW-068-investigate-an-api-gateway-request-failure.md) | Junior |
| 069 | [Diagnose unhealthy ALB targets](cloud/aws/applications/DIW-069-diagnose-unhealthy-alb-targets.md) | Mid-Level |
| 070 | [Repair Lambda access to DynamoDB](cloud/aws/applications/DIW-070-repair-lambda-access-to-dynamodb.md) | Mid-Level |
| 071 | [Investigate a private application across VPC ALB and DNS boundaries](cloud/aws/applications/DIW-071-investigate-a-private-application-across-vpc-alb-and-dns-boundaries.md) | Senior |
| 072 | [Diagnose EKS workload identity and cloud access failures](cloud/aws/applications/DIW-072-diagnose-eks-workload-identity-and-cloud-access-failures.md) | Senior |

### Azure

| # | Interview question | Difficulty |
|---|---|---|
| 073 | [Diagnose a VM connection failure](cloud/azure/DIW-073-diagnose-a-vm-connection-failure.md) | Junior |
| 074 | [Verify a managed identity resource assignment](cloud/azure/DIW-074-verify-a-managed-identity-resource-assignment.md) | Junior |
| 075 | [Repair AKS image pulls from ACR](cloud/azure/DIW-075-repair-aks-image-pulls-from-acr.md) | Mid-Level |
| 076 | [Investigate Azure private DNS resolution](cloud/azure/DIW-076-investigate-azure-private-dns-resolution.md) | Mid-Level |
| 077 | [Trace an application failure across Azure load balancing and networking](cloud/azure/DIW-077-trace-an-application-failure-across-azure-load-balancing-and-networking.md) | Senior |
| 078 | [Diagnose AKS access to a private Azure dependency](cloud/azure/DIW-078-diagnose-aks-access-to-a-private-azure-dependency.md) | Senior |

### Google Cloud

| # | Interview question | Difficulty |
|---|---|---|
| 079 | [Diagnose Compute Engine connectivity](cloud/gcp/DIW-079-diagnose-compute-engine-connectivity.md) | Junior |
| 080 | [Inspect Artifact Registry access](cloud/gcp/DIW-080-inspect-artifact-registry-access.md) | Junior |
| 081 | [Repair a Cloud Run startup failure](cloud/gcp/DIW-081-repair-a-cloud-run-startup-failure.md) | Mid-Level |
| 082 | [Investigate GKE workload access to a cloud service](cloud/gcp/DIW-082-investigate-gke-workload-access-to-a-cloud-service.md) | Mid-Level |
| 083 | [Trace private Google Cloud application connectivity](cloud/gcp/DIW-083-trace-private-google-cloud-application-connectivity.md) | Senior |
| 084 | [Diagnose Cloud Run latency under concurrency and dependency pressure](cloud/gcp/DIW-084-diagnose-cloud-run-latency-under-concurrency-and-dependency-pressure.md) | Senior |

### Terraform

| # | Interview question | Difficulty |
|---|---|---|
| 085 | [Inspect a plan before changing infrastructure](terraform/DIW-085-inspect-a-plan-before-changing-infrastructure.md) | Junior |
| 086 | [Diagnose an invalid variable or provider configuration](terraform/DIW-086-diagnose-an-invalid-variable-or-provider-configuration.md) | Junior |
| 087 | [Investigate drift before applying changes](terraform/DIW-087-investigate-drift-before-applying-changes.md) | Mid-Level |
| 088 | [Recover from a failed partial apply](terraform/DIW-088-recover-from-a-failed-partial-apply.md) | Mid-Level |
| 089 | [Refactor resource addresses without recreation](terraform/DIW-089-refactor-resource-addresses-without-recreation.md) | Senior |
| 090 | [Recover inaccessible state using a documented backend recovery procedure](terraform/DIW-090-recover-inaccessible-state-using-a-documented-backend-recovery-procedure.md) | Senior |

### Ansible

| # | Interview question | Difficulty |
|---|---|---|
| 091 | [Fix an inventory targeting error](ansible/DIW-091-fix-an-inventory-targeting-error.md) | Junior |
| 092 | [Diagnose privilege escalation failure](ansible/DIW-092-diagnose-privilege-escalation-failure.md) | Junior |
| 093 | [Repair a non-idempotent playbook](ansible/DIW-093-repair-a-non-idempotent-playbook.md) | Mid-Level |
| 094 | [Handle rolling changes with health verification](ansible/DIW-094-handle-rolling-changes-with-health-verification.md) | Mid-Level |
| 095 | [Recover from a partially completed configuration rollout](ansible/DIW-095-recover-from-a-partially-completed-configuration-rollout.md) | Senior |
| 096 | [Prevent secret disclosure through tasks and logs](ansible/DIW-096-prevent-secret-disclosure-through-tasks-and-logs.md) | Senior |

### Jenkins

| # | Interview question | Difficulty |
|---|---|---|
| 097 | [Fix a pipeline syntax error](ci-cd/jenkins/DIW-097-fix-a-pipeline-syntax-error.md) | Junior |
| 098 | [Diagnose a missing build tool on an agent](ci-cd/jenkins/DIW-098-diagnose-a-missing-build-tool-on-an-agent.md) | Junior |
| 099 | [Investigate workspace permission failures](ci-cd/jenkins/DIW-099-investigate-workspace-permission-failures.md) | Mid-Level |
| 100 | [Repair artifact handoff between stages](ci-cd/jenkins/DIW-100-repair-artifact-handoff-between-stages.md) | Mid-Level |
| 101 | [Diagnose a pipeline that fails only under concurrent builds](ci-cd/jenkins/DIW-101-diagnose-a-pipeline-that-fails-only-under-concurrent-builds.md) | Senior |
| 102 | [Implement and verify recovery after a failed deployment](ci-cd/jenkins/DIW-102-implement-and-verify-recovery-after-a-failed-deployment.md) | Senior |

### GitHub Actions

| # | Interview question | Difficulty |
|---|---|---|
| 103 | [Fix a workflow trigger that does not run](ci-cd/github-actions/DIW-103-fix-a-workflow-trigger-that-does-not-run.md) | Junior |
| 104 | [Preserve useful output from a failing test job](ci-cd/github-actions/DIW-104-preserve-useful-output-from-a-failing-test-job.md) | Junior |
| 105 | [Repair cross-job artifact handoff](ci-cd/github-actions/DIW-105-repair-cross-job-artifact-handoff.md) | Mid-Level |
| 106 | [Diagnose a failing matrix build](ci-cd/github-actions/DIW-106-diagnose-a-failing-matrix-build.md) | Mid-Level |
| 107 | [Secure cloud deployment with scoped OIDC permissions](ci-cd/github-actions/DIW-107-secure-cloud-deployment-with-scoped-oidc-permissions.md) | Senior |
| 108 | [Diagnose deployment races and prevent stale releases](ci-cd/github-actions/DIW-108-diagnose-deployment-races-and-prevent-stale-releases.md) | Senior |

### GitLab and Azure pipelines

| # | Interview question | Difficulty |
|---|---|---|
| 109 | [Fix a GitLab job excluded by rules](ci-cd/gitlab-and-azure/DIW-109-fix-a-gitlab-job-excluded-by-rules.md) | Junior |
| 110 | [Diagnose an Azure Pipeline agent capability mismatch](ci-cd/gitlab-and-azure/DIW-110-diagnose-an-azure-pipeline-agent-capability-mismatch.md) | Junior |
| 111 | [Repair a GitLab deployment image tag](ci-cd/gitlab-and-azure/DIW-111-repair-a-gitlab-deployment-image-tag.md) | Mid-Level |
| 112 | [Diagnose Azure environment permissions and approvals](ci-cd/gitlab-and-azure/DIW-112-diagnose-azure-environment-permissions-and-approvals.md) | Mid-Level |
| 113 | [Recover a GitLab release with failed verification](ci-cd/gitlab-and-azure/DIW-113-recover-a-gitlab-release-with-failed-verification.md) | Senior |
| 114 | [Recover an Azure deployment with failed verification](ci-cd/gitlab-and-azure/DIW-114-recover-an-azure-deployment-with-failed-verification.md) | Senior |

### GitOps

| # | Interview question | Difficulty |
|---|---|---|
| 115 | [Find an Argo CD application sync error](gitops/DIW-115-find-an-argo-cd-application-sync-error.md) | Junior |
| 116 | [Inspect a failed Flux reconciliation](gitops/DIW-116-inspect-a-failed-flux-reconciliation.md) | Junior |
| 117 | [Diagnose repeated Argo CD drift](gitops/DIW-117-diagnose-repeated-argo-cd-drift.md) | Mid-Level |
| 118 | [Repair a Flux source or dependency failure](gitops/DIW-118-repair-a-flux-source-or-dependency-failure.md) | Mid-Level |
| 119 | [Recover a release when automated reconciliation reapplies a bad change](gitops/DIW-119-recover-a-release-when-automated-reconciliation-reapplies-a-bad-change.md) | Senior |
| 120 | [Diagnose conflicting controllers managing the same resource](gitops/DIW-120-diagnose-conflicting-controllers-managing-the-same-resource.md) | Senior |

### Metrics

| # | Interview question | Difficulty |
|---|---|---|
| 121 | [Restore a missing Prometheus scrape target](observability/metrics/DIW-121-restore-a-missing-prometheus-scrape-target.md) | Junior |
| 122 | [Fix a Grafana data source connection](observability/metrics/DIW-122-fix-a-grafana-data-source-connection.md) | Junior |
| 123 | [Diagnose missing metrics caused by label selection](observability/metrics/DIW-123-diagnose-missing-metrics-caused-by-label-selection.md) | Mid-Level |
| 124 | [Correct a misleading request error rate query](observability/metrics/DIW-124-correct-a-misleading-request-error-rate-query.md) | Mid-Level |
| 125 | [Investigate high metric cardinality and ingestion pressure](observability/metrics/DIW-125-investigate-high-metric-cardinality-and-ingestion-pressure.md) | Senior |
| 126 | [Build and verify an SLO burn rate view from service metrics](observability/metrics/DIW-126-build-and-verify-an-slo-burn-rate-view-from-service-metrics.md) | Senior |

### Logs

| # | Interview question | Difficulty |
|---|---|---|
| 127 | [Find logs using service labels and time ranges](observability/logs/DIW-127-find-logs-using-service-labels-and-time-ranges.md) | Junior |
| 128 | [Diagnose a log collector permission failure](observability/logs/DIW-128-diagnose-a-log-collector-permission-failure.md) | Junior |
| 129 | [Trace missing logs through Fluent Bit and Loki](observability/logs/DIW-129-trace-missing-logs-through-fluent-bit-and-loki.md) | Mid-Level |
| 130 | [Repair a Fluentd or Logstash parsing failure](observability/logs/DIW-130-repair-a-fluentd-or-logstash-parsing-failure.md) | Mid-Level |
| 131 | [Investigate Elasticsearch ingestion rejection and backlog](observability/logs/DIW-131-investigate-elasticsearch-ingestion-rejection-and-backlog.md) | Senior |
| 132 | [Preserve log delivery during downstream failure and recovery](observability/logs/DIW-132-preserve-log-delivery-during-downstream-failure-and-recovery.md) | Senior |

### Tracing and alerting

| # | Interview question | Difficulty |
|---|---|---|
| 133 | [Find a request trace and inspect its spans](observability/traces-and-alerting/DIW-133-find-a-request-trace-and-inspect-its-spans.md) | Junior |
| 134 | [Inspect alert state and notification routing](observability/traces-and-alerting/DIW-134-inspect-alert-state-and-notification-routing.md) | Junior |
| 135 | [Repair an OpenTelemetry export failure](observability/traces-and-alerting/DIW-135-repair-an-opentelemetry-export-failure.md) | Mid-Level |
| 136 | [Diagnose an Alertmanager notification that never arrives](observability/traces-and-alerting/DIW-136-diagnose-an-alertmanager-notification-that-never-arrives.md) | Mid-Level |
| 137 | [Restore cross-service trace context propagation](observability/traces-and-alerting/DIW-137-restore-cross-service-trace-context-propagation.md) | Senior |
| 138 | [Diagnose alert storms and validate grouping inhibition and recovery](observability/traces-and-alerting/DIW-138-diagnose-alert-storms-and-validate-grouping-inhibition-and-recovery.md) | Senior |

### Cloud and commercial telemetry

| # | Interview question | Difficulty |
|---|---|---|
| 139 | [Find application logs in CloudWatch](observability/cloud-and-commercial/DIW-139-find-application-logs-in-cloudwatch.md) | Junior |
| 140 | [Query workload logs in Google Cloud Logging](observability/cloud-and-commercial/DIW-140-query-workload-logs-in-google-cloud-logging.md) | Junior |
| 141 | [Diagnose missing Azure Monitor application telemetry](observability/cloud-and-commercial/DIW-141-diagnose-missing-azure-monitor-application-telemetry.md) | Mid-Level |
| 142 | [Repair missing Datadog service telemetry](observability/cloud-and-commercial/DIW-142-repair-missing-datadog-service-telemetry.md) | Mid-Level |
| 143 | [Investigate inconsistent latency measurements across New Relic instrumentation](observability/cloud-and-commercial/DIW-143-investigate-inconsistent-latency-measurements-across-new-relic-instrumentation.md) | Senior |
| 144 | [Correlate cloud telemetry and application evidence during a service outage](observability/cloud-and-commercial/DIW-144-correlate-cloud-telemetry-and-application-evidence-during-a-service-outage.md) | Senior |

### Security automation and combined incidents

| # | Interview question | Difficulty |
|---|---|---|
| 145 | [Scan a container image and interpret findings](combined-scenarios/DIW-145-scan-a-container-image-and-interpret-findings.md) | Junior |
| 146 | [Write a Python health check with explicit timeout and exit behavior](combined-scenarios/DIW-146-write-a-python-health-check-with-explicit-timeout-and-exit-behavior.md) | Junior |
| 147 | [Replace broad workload permissions and verify behavior](combined-scenarios/DIW-147-replace-broad-workload-permissions-and-verify-behavior.md) | Mid-Level |
| 148 | [Automate collection of redacted incident evidence](combined-scenarios/DIW-148-automate-collection-of-redacted-incident-evidence.md) | Mid-Level |
| 149 | [Investigate a failed release across pipelines containers metrics logs and traces](combined-scenarios/DIW-149-investigate-a-failed-release-across-pipelines-containers-metrics-logs-and-traces.md) | Senior |
| 150 | [Recover a compromised workload while preserving evidence and restoring service](combined-scenarios/DIW-150-recover-a-compromised-workload-while-preserving-evidence-and-restoring-service.md) | Senior |

## How to practice

1. Choose a question and read its difficulty and tool requirements.
2. Explain your approach before looking up commands.
3. Separate observations, hypotheses, and proposed changes.
4. Describe how you would verify recovery and prevent recurrence.
5. Record gaps in your answer and revisit them after practice.

## Exercise walkthroughs

As full exercises are released, their question files will gain setup assets, optional hints, investigation commands, root-cause explanations, solutions, verification, cleanup, and follow-up answer points. Video links will appear when recordings exist.

## About the questions

These are original educational prompts. They are not attributed to company interviews. Tool groups identify coverage; each future lab will specify its exact implementation, versions, account requirements, and costs.

## VERIQTA

Build your technical understanding through practical investigation and clear engineering explanations.

Star DevOps Interview World if it helps your preparation.
