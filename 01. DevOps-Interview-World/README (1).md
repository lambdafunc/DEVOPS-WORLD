# DevOps Interview World

Practical DevOps interview preparation by VERIQTA. Learn to investigate failures, explain engineering decisions, and demonstrate recovery through hands-on scenarios across infrastructure, containers, cloud platforms, delivery pipelines, security, and observability.

Whether you are preparing for your first DevOps role or a senior technical interview, practice showing how you reached your answer. A working command matters. So do the evidence behind it, the risks of the change, and the checks that prove the problem is resolved.

## Repository status

This repository is under construction. The coverage and publication standard below define the initial scope. Scenario guides and runnable assets will be published progressively. No scenarios or videos are claimed as completed in this initial edition.

## Start here

1. Choose a tool area from the coverage table.
2. Choose a scenario appropriate to your experience.
3. Read its prerequisites and environment requirements before running commands.
4. Attempt the task before opening the guided solution.
5. Record your evidence, verify the result, and clean up the environment.
6. Practice explaining your investigation and decisions aloud.

## Tools and coverage

| Area | Tools and subjects | Interview practice |
|---|---|---|
| Linux | Processes, systemd, permissions, storage, packages, logs | Diagnose service failures, resource pressure, and access problems |
| Shell automation | Bash, core utilities | Write reliable scripts and handle failures |
| Version control | Git, GitHub | Resolve conflicts, recover commits, and manage changes |
| Networking | DNS, routing, TCP/IP, HTTP, HTTPS, TLS, Nginx | Trace connectivity failures and request paths |
| Container engines and runtimes | Docker, Podman, containerd, CRI-O | Investigate startup failures, runtime behavior, and isolation |
| Container builds | Dockerfiles, BuildKit, Buildx, Docker Compose | Build images, diagnose builds, and handle multiple architectures |
| Container registries | Docker Hub, Amazon ECR, Azure ACR, Google Artifact Registry | Diagnose authentication, image distribution, and tagging problems |
| Kubernetes | Workloads, Services, ingress, storage, scheduling, RBAC | Investigate failed workloads and recover service traffic |
| Kubernetes configuration | Helm, Kustomize | Diagnose rendering, configuration, and release problems |
| AWS | IAM, VPC, EC2, ALB, Route 53, S3, Lambda, API Gateway, DynamoDB, EKS | Build and troubleshoot cloud infrastructure |
| Azure | Identity, networking, compute, AKS, Azure DevOps | Investigate infrastructure and delivery failures |
| Google Cloud | IAM, networking, Compute Engine, GKE, Cloud Run | Investigate access, workload, and connectivity failures |
| Infrastructure as code | Terraform | Review plans, troubleshoot state, and manage drift |
| Configuration management | Ansible | Diagnose inventory, privilege, and idempotency problems |
| CI/CD | Jenkins, GitHub Actions, GitLab CI/CD, Azure Pipelines | Investigate failed builds, tests, deployments, and artifact handoffs |
| GitOps | Argo CD, Flux | Diagnose reconciliation and deployment drift |
| Metrics and dashboards | Prometheus, Grafana | Investigate scrape failures, misleading queries, and missing metrics |
| Logs | Loki, Fluent Bit, Fluentd, Elasticsearch, Logstash, Kibana | Trace missing logs and diagnose collection and query problems |
| Tracing | OpenTelemetry, Jaeger, Tempo | Investigate missing spans and trace requests across services |
| Alerting | Alertmanager, Grafana Alerting | Diagnose missing notifications, routing, and noisy alerts |
| Cloud observability | CloudWatch, Azure Monitor, Google Cloud Monitoring and Logging | Correlate platform telemetry with application failures |
| Commercial observability | Datadog, New Relic | Investigate instrumentation, ingestion, and alerting problems |
| Security | Trivy, secrets, least privilege, image and runtime hardening | Identify exposure, reduce access, and validate remediation |
| Python automation | APIs, structured data, subprocesses, error handling | Automate operational tasks with clear failure behavior |
| Combined scenarios | Multiple tools from the areas above | Follow failures across application and infrastructure boundaries |

Coverage is a publication plan. Each scenario will identify the specific tools it uses, required versions, and any account or subscription requirements.

## Difficulty guide

| Level | What you practice | What a strong answer demonstrates |
|---|---|---|
| Junior | Bounded tasks and common failures in one tool | Correct commands, clear explanations, and basic verification |
| Mid-Level | Failures spanning several components | Structured investigation, evidence, and safe recovery |
| Senior | Ambiguous incidents and operational tradeoffs | Prioritization, risk management, recovery strategy, and prevention |

Difficulty reflects the reasoning and operational responsibility required, not just the number of commands.

## Scenario catalogue

The catalogue will list published scenarios using the following fields. Add a guide link only when its file exists. Add a video link only when the recording is available.

| ID | Scenario | Tools | Difficulty | Guide | Video |
|---|---|---|---|---|---|

Published scenarios: 0.

Scenarios are original educational exercises unless an attribution explicitly states otherwise. Company interview associations will be included only when supported by a cited source. Educational lab environments simulate operational problems; they do not establish that a scenario occurred at a named company.

## What each scenario includes

- A realistic problem statement, symptoms, and success criteria.
- Prerequisites, supported versions, and environment requirements.
- Setup instructions and the files needed to reproduce the task.
- An independent attempt section with optional hints.
- A guided investigation explaining commands and evidence.
- Root cause and a complete solution.
- Expected results, including notes about environment-dependent output.
- Verification that checks both recovery and relevant failure behavior.
- Troubleshooting for common lab problems.
- Cleanup or reset instructions, including cloud resources that incur charges.
- Interview follow-up questions and suggested answer points.
- Prevention and engineering tradeoffs where relevant.
- Sources and an honest statement of validation performed.

## Repository organization

Use one root README as the central index. Each scenario has one Markdown guide. Supporting files live beside it only when the exercise needs them.

| Planned folder | Contents |
|---|---|
| `linux/` | Linux scenarios |
| `bash/` | Shell automation scenarios |
| `git/` | Version control scenarios |
| `networking/` | Networking and web traffic scenarios |
| `containers/` | Engines, runtimes, builds, Compose, and registries |
| `kubernetes/` | Kubernetes, Helm, and Kustomize scenarios |
| `cloud/aws/` | AWS scenarios |
| `cloud/azure/` | Azure scenarios |
| `cloud/gcp/` | Google Cloud scenarios |
| `terraform/` | Infrastructure as code scenarios |
| `ansible/` | Configuration management scenarios |
| `ci-cd/` | Pipeline scenarios |
| `gitops/` | Argo CD and Flux scenarios |
| `observability/metrics/` | Prometheus and Grafana scenarios |
| `observability/logs/` | Log collection, storage, and query scenarios |
| `observability/traces/` | OpenTelemetry and distributed tracing scenarios |
| `observability/alerting/` | Alert evaluation, routing, and notification scenarios |
| `observability/cloud/` | Cloud-native observability scenarios |
| `observability/commercial/` | Datadog and New Relic scenarios |
| `security/` | Security scenarios |
| `python/` | Python automation scenarios |
| `combined-scenarios/` | Scenarios involving several tools |

Scenario IDs use one global sequence, starting at `DIW-001`. Guide filenames use the ID followed by a descriptive lowercase slug. For example, `DIW-001-service-fails-after-restart.md`. Supporting assets use the same stem as their guide. Paths, resource names, and commands must agree throughout each exercise.

## Practice for the interview

For each scenario, explain the following in your own words.

1. What failed, and what was the impact?
2. What did you check first, and why?
3. Which evidence supported or ruled out each hypothesis?
4. What change did you make, and what risk did it introduce?
5. How did you verify recovery?
6. How would you prevent or detect a recurrence?

Keep a short record of commands, observations, and decisions. Remove credentials, tokens, account details, and personal information before sharing your work.

## Publication standard

Every published scenario must have internally consistent commands and assets, working relative links, explicit prerequisites, and usable cleanup instructions. Guides must distinguish checks that were actually executed from documentation review and steps that still require validation.

Cloud, commercial, and privileged exercises must explain their environment requirements before setup. Use isolated lab environments and inspect changes before applying them.

## About VERIQTA

VERIQTA creates practical engineering learning resources that connect technical knowledge with investigation, implementation, and verification.

If this repository helps your preparation, star it and share it with another engineer.
