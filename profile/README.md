# DecafAI - Your AI DevOps Engineer | https://decafai.dev

<div align="center">
  
  ![DecafAI Logo](https://avatars.githubusercontent.com/u/218587052)
  
  **Automate. Secure. Deploy. Sleep.**
  
  [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
  [![Status](https://img.shields.io/badge/Status-Active_Development-green.svg)]()
  [![Community](https://img.shields.io/badge/Join-Community-purple.svg)](https://github.com/decafaihq/decafai/discussions)

  <br>
  
</div>
---

##  What is DecafAI?

DecafAI is your 24/7 AI-powered DevOps engineer that writes Infrastructure as Code, fixes CI/CD pipelines, patches vulnerabilities, and handles infrastructure tasks while you focus on building. It's not another dashboard - it creates actual pull requests, writes real fixes, and delivers working code.

### Key Features

- **🏗️ Infrastructure as Code Writer** - Generates production-ready Terraform modules, Ansible playbooks, and Kubernetes manifests
- **🔧 CI/CD Pipeline Doctor** - Debugs failed builds, optimizes slow pipelines, and writes GitHub Actions/GitLab CI/Jenkins workflows
- **🛡️ Security Vulnerability Fixer** - Scans for CVEs, generates patches, updates dependencies, and creates security policies
- **🚀 Deployment Automator** - Handles blue-green deployments, canary releases, and rollbacks with zero downtime
- **🐛 Incident Responder** - Investigates issues, finds root causes, and generates fixes when things break
- **📚 Documentation Generator** - Writes README files, API docs, runbooks, and architecture diagrams

## How It Works

DecafAI leverages advanced AI models to understand your infrastructure, analyze problems, and generate solutions. The Community Edition uses **Mixtral-8×7B** as the default model, providing an excellent blend of speed, size, and license freedom for most DevOps tasks.

```bash
$ kubectl get pods | grep crash
api-gateway-7f9c5c4b5d-x2j4k    0/1     CrashLoopBackOff   12    36m

$ decaf diagnose pod/api-gateway --fix
🔍 Analyzing crash patterns...
⚠️  Root Cause: OOMKilled - memory leak in v2.3.1
📋 Proposed Fix:
   - Update image to v2.3.2 (fixes memory leak)
   - Increase memory limit from 512Mi to 1Gi
   - Add liveness probe with memory threshold
🤔 Apply these fixes and create PR? [y/N]: y
✅ Created PR #247: Fix api-gateway OOMKill issue
🔗 https://github.com/org/repo/pull/247
```

###  AI Model Architecture

**Default Model (CE):** Mixtral-8×7B
- Fast inference for real-time DevOps tasks
- Runs efficiently on standard hardware
- Apache 2.0 licensed - truly open

**Plug-in Architecture:** Easily swap models without code changes
```yaml
# config/decafai.yaml
ai:
  model: mixtral-8x7b  # Default
  # model: llama-3-70b     # For deeper reasoning
  # model: dbrx            # For complex analysis
  # model: qwen-2-72b      # Alternative option
```

Power users and Enterprise deployments can scale reasoning depth by plugging in larger models like Llama-3-70B, DBRX, or Qwen-2-72B for more complex scenarios.

## Deep Integrations

DecafAI integrates deeply with your existing DevOps stack:

<table>
<tr>
<td><b>Infrastructure</b></td>
<td><b>CI/CD</b></td>
<td><b>Security</b></td>
<td><b>Cloud</b></td>
</tr>
<tr>
<td>

- Terraform
- Ansible
- Kubernetes
- Helm
- Docker/Podman

</td>
<td>

- GitHub Actions
- GitLab CI
- Jenkins
- CircleCI
- ArgoCD/FluxCD

</td>
<td>

- Trivy
- Vault
- OWASP Tools
- Snyk
- Prometheus/Grafana

</td>
<td>

- AWS
- Azure
- GCP
- On-premise
- Hybrid

</td>
</tr>
</table>

## Deployment Options

### Openssource Edition
```bash
# Quick start (coming soon)
git clone https://github.com/decafaihq/decafai
cd decafai
./install.sh
```

**Features:**
- ✅ Full DevOps automation capabilities
- ✅ DevSecOps features
- ✅ Self-hosted on your infrastructure
- ✅ Air-gapped deployment support
- ✅ Apache 2.0 license
- ✅ Community support
- ✅ **Mixtral-8×7B** included (default model)
- ✅ Plug-in support for Llama-3-70B, DBRX, Qwen-2-72B


## Project Status

DecafAI is in **active development**. We're building in the open and welcome contributions!

### Current Focus Areas:
- [ ] Core AI engine with Mixtral-8×7B integration
- [ ] Plug-in architecture for model swapping
- [ ] Terraform module generation
- [ ] Kubernetes manifest creation
- [ ] CI/CD pipeline optimization
- [ ] Security vulnerability detection and patching
- [ ] Documentation generation

## Contributing

We love contributions! Whether you're fixing bugs, adding features, or improving documentation, we'd love to have you as part of the DecafAI community.

email us at hello@decafai.dev




## 📊 Why DecafAI?

### The Problem
- **70% of DevOps time** is spent on repetitive toil
- **3 AM incidents** require immediate response
- **Security vulnerabilities** need constant patching
- **Documentation** is always outdated

### The Solution
DecafAI handles the toil so you can:
- 📈 Reduce operational overhead by 70%
- 🛌 Sleep through the night (DecafAI handles incidents)
- 🔒 Maintain security compliance automatically
- 📚 Keep documentation always up-to-date

## 🗺️ Roadmap

### Phase 1: Foundation (Current)
- Core AI integration with Mistral/Codestral
- Basic IaC generation
- Simple CI/CD fixes

### Phase 2: Intelligence (Q2 2025)
- Advanced pattern learning from your codebase
- Predictive incident prevention
- Custom model fine-tuning

### Phase 3: Autonomy (Q3 2025)
- Full autonomous operations mode
- Self-healing infrastructure
- Proactive optimization

## 💬 Community

Join our growing community of DevOps engineers automating away the toil:

- **[GitHub Discussions](https://github.com/decafaihq/decafai/discussions)** - Ask questions, share ideas -- Coming Soon !  Email us for now !


## 📄 License

DecafAI Community Edition is licensed under the [Apache License 2.0](LICENSE).

## 🙏 Acknowledgments

Built with ❤️ by the community
---

<div align="center">
  
**Stop Fighting Fires. Start Building.**

[Get Started](https://github.com/decafaihq/decafai) • [Documentation](https://docs.decafai.dev) • [Community](https://github.com/decafaihq/decafai/discussions)

</div>
