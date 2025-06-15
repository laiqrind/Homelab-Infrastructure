# Homelab Infrastructure Project

<div align="center">

![Project Status](https://img.shields.io/badge/Status-In%20Development-orange)
![License](https://img.shields.io/badge/License-MIT-blue)
<!--![GitHub Issues](https://img.shields.io/github/issues/yourusername/homelab-infrastructure)
![GitHub Stars](https://img.shields.io/github/stars/yourusername/homelab-infrastructure)-->
![Uptime](https://img.shields.io/badge/Planned%20Uptime-99.9%25-green)

</div>

<table border="0px">
  <tr>
    <td>
      <img src="https://github.com/laiqrind/Homelab-Infrastructure/assets/images/9FD5399E-4D3C-41BE-93B3-5777E1659411.png" alt="Enterprise homelab rack infrastructure icon" width="150" height="120"/>
    </td>
    <td>
      <h2>🏗️ Enterprise-Grade Homelab Infrastructure</h2>
      <p><strong>Professional self-hosted infrastructure</strong> built with Raspberry Pi 500, enterprise load balancing, monitoring stack, and container orchestration. This project demonstrates production-level DevOps practices with <strong>zero recurring hosting costs</strong> while providing $3,000+/year equivalent cloud infrastructure value.</p>
      
      <p>🎯 <strong>Mission:</strong> Build a complete enterprise-grade homelab that serves as both a learning platform and production-ready infrastructure for personal projects.</p>
    </td>
  </tr>
</table>

---

## 📊 Project Overview

| **Component** | **Technology** | **Purpose** | **Status** |
|---------------|----------------|-------------|------------|
| **Primary Dashboard** | Raspberry Pi 500 + Node.js | Main application server | 🟡 Planning |
| **Load Balancer** | Homelab1 + HAProxy | Traffic distribution & SSL | 🟡 Planning |
| **Monitoring Stack** | Homelab2 + Prometheus/Grafana | Observability & alerts | 🟡 Planning |
| **CI/CD Pipeline** | Homelab3 + GitLab/Jenkins | Automated deployments | 🟡 Planning |
| **Container Platform** | Pi Cluster + Kubernetes | Microservices orchestration | 🟡 Planning |
| **Storage** | NAS + pCloud (10TB) + Mega (2TB) | Distributed file storage | 🟡 Planning |
| **Public Portfolio** | GitHub Pages + Cloudflare | Professional website | 🟡 Planning |

---

## 🏗️ Infrastructure Architecture

### **Physical Setup: Samson SRK16 16U Rack**
```
┌─────────────────────────────────────────────┐
│  🖥️  Raspberry Pi 500 Desktop (On Top)     │
├─────────────────────────────────────────────┤
│ 16U │  📦  NAS Storage (Future)            │
│ 15U │                                      │
├─────────────────────────────────────────────┤
│ 14U │  🐳  Pi Cluster (Kubernetes)         │
│ 13U │                                      │
├─────────────────────────────────────────────┤
│ 12U │  💻  Homelab3    💻  Homelab2       │
│ 11U │  (CI/CD)        (Monitoring)        │
├─────────────────────────────────────────────┤
│ 10U │  ⚖️   Homelab1 (Load Balancer)      │
│  9U │                                      │
│  8U │                                      │
├─────────────────────────────────────────────┤
│7-2U │  📈  Future Expansion Space          │
├─────────────────────────────────────────────┤
│ 1U  │  🔋  UPS Power Management (Future)   │
└─────────────────────────────────────────────┘
```

### **Network Flow**
```
Internet → Router → Homelab1 (HAProxy) → Raspberry Pi 500 (App)
                                       ↓
                                 Pi Cluster (Containers)
```

---

## 💻 Technology Stack

### **Frontend Technologies**
- **Static Sites:** HTML5, CSS3, JavaScript (ES6+)
- **Framework:** TailwindCSS / Bootstrap
- **Build Tools:** GitHub Actions, Webpack/Vite
- **Hosting:** GitHub Pages + Cloudflare

### **Backend Technologies**  
- **Runtime:** Node.js 18 LTS
- **Framework:** Express.js
- **Database:** SQLite (primary), PostgreSQL (secondary)
- **Authentication:** JWT + Passport.js
- **File Storage:** pCloud Drive (local mount)

### **Infrastructure & DevOps**
- **Load Balancer:** HAProxy + Nginx
- **Container Platform:** Kubernetes / Docker Swarm
- **Monitoring:** Prometheus + Grafana + AlertManager
- **Logging:** ELK Stack (Elasticsearch, Logstash, Kibana)
- **CI/CD:** GitLab CE / Jenkins
- **Security:** Let's Encrypt SSL, fail2ban, UFW

### **Hardware Stack**
- **Primary:** Raspberry Pi 500 (8GB RAM, ARM Cortex-A76)
- **Servers:** 3x Lenovo Small Form Factor machines
- **Cluster:** 4x Raspberry Pi (Kubernetes nodes)
- **Storage:** 10TB pCloud + 2TB Mega cloud integration
- **Network:** Gigabit Ethernet, managed switch
- **Rack:** Samson SRK16 16U Universal Rack Stand

---

## ✨ Key Features

### **🌐 Public Portfolio**
- Professional developer portfolio on `laiqrind.dev` & `laiqrind.net`
- Responsive design with modern UI/UX
- SEO optimized with social media integration
- Automated deployment via GitHub Actions

### **🏠 Private Dashboard**  
- Personal productivity workspace
- To-do list and calendar management
- Email integration and notifications
- File management with cloud storage sync

### **⚖️ High Availability**
- Load balancing across multiple nodes
- Health checks and automatic failover
- SSL termination and certificate automation
- <30 second recovery time for critical services

### **📊 Enterprise Monitoring**
- Real-time infrastructure monitoring
- Application performance metrics
- Log aggregation and analysis
- Custom dashboards and alerting

### **🐳 Container Orchestration**
- Kubernetes cluster on Raspberry Pi hardware
- Microservices architecture
- Auto-scaling and service discovery
- GitOps deployment workflows

### **🔒 Security & Compliance**
- Multi-layer security architecture
- Automated security updates
- Network segmentation and firewalls
- Secure remote access via VPN

---

## 📈 Cost Analysis

### **Annual Cost Comparison**
| **Component** | **Homelab Cost** | **AWS Equivalent** | **Annual Savings** |
|---------------|------------------|--------------------|--------------------|
| **Load Balancer** | $0 | $200/year | $200 |
| **3x App Servers** | $0 | $1,800/year | $1,800 |
| **Database** | $0 | $600/year | $600 |
| **Monitoring** | $0 | $300/year | $300 |
| **Storage** | $0* | $400/year | $400 |
| **SSL & CDN** | $0 | $120/year | $120 |
| **Total Annual** | **~$100*** | **$3,420** | **$3,320** |

*\*Using existing pCloud/Mega lifetime subscriptions*  
*\*\*Electricity costs only*

### **Learning Value**
- **DevOps Skills:** $80k-120k salary equivalent knowledge
- **Cloud Architecture:** Enterprise-level design patterns
- **Container Orchestration:** Kubernetes certification preparation
- **Monitoring & Observability:** Production SRE experience

---

## 🚀 Quick Start

### **Prerequisites**
- Raspberry Pi 500 with latest Pi OS
- Domain names registered with Cloudflare
- GitHub Individual account
- Basic networking knowledge

### **Phase 1: Foundation Setup**
```bash
# Clone the repository
git clone https://github.com/yourusername/homelab-infrastructure.git
cd homelab-infrastructure

# Set up development environment
./scripts/setup-dev-environment.sh

# Configure initial infrastructure
./scripts/setup-pi500.sh
```

### **Phase 2: Deploy Portfolio**
```bash
# Deploy static portfolio to GitHub Pages
./scripts/deploy-portfolio.sh

# Configure custom domains
./scripts/configure-domains.sh
```

### **Phase 3: Infrastructure Deployment**
```bash
# Set up load balancer (Homelab1)
./scripts/setup-load-balancer.sh

# Deploy monitoring stack (Homelab2)
./scripts/setup-monitoring.sh

# Configure CI/CD pipeline (Homelab3)
./scripts/setup-cicd.sh
```

---

## 📋 Project Milestones

### **🏗️ Phase 1: Foundation (Weeks 1-2)**
- [x] ~~Development environment setup~~
- [ ] Domain configuration (laiqrind.dev, laiqrind.net)
- [ ] GitHub repository structure
- [ ] Basic security hardening

### **🌐 Phase 2: Portfolio Deployment (Weeks 3-4)**
- [ ] Static portfolio development
- [ ] Responsive design implementation
- [ ] CI/CD pipeline setup
- [ ] SEO and performance optimization

### **🖥️ Phase 3: Primary Dashboard (Weeks 5-6)**
- [ ] Raspberry Pi 500 configuration
- [ ] Node.js application development
- [ ] pCloud Drive integration
- [ ] Authentication system

### **⚖️ Phase 4: Load Balancing (Weeks 7-8)**
- [ ] Homelab1 server setup
- [ ] HAProxy configuration
- [ ] SSL certificate automation
- [ ] High availability testing

### **📊 Phase 5: Monitoring & CI/CD (Weeks 9-10)**
- [ ] Prometheus + Grafana setup
- [ ] ELK stack deployment
- [ ] GitLab/Jenkins configuration
- [ ] Automated testing pipeline

### **🐳 Phase 6: Container Orchestration (Weeks 11-12)**
- [ ] Kubernetes cluster setup
- [ ] Application containerization
- [ ] Service mesh implementation
- [ ] Production deployment

**Current Progress:** 🟡 Phase 1 - Foundation Setup

---

## 📁 Repository Structure

```
homelab-infrastructure/
├── 📁 docs/                    # Documentation and guides
│   ├── architecture.md         # System architecture details
│   ├── setup-guides/          # Step-by-step setup instructions
│   └── troubleshooting.md     # Common issues and solutions
├── 📁 scripts/                 # Automation scripts
│   ├── setup-dev-environment.sh
│   ├── deploy-portfolio.sh
│   └── backup-configs.sh
├── 📁 portfolio/              # Static portfolio website
│   ├── src/                   # Source files
│   ├── dist/                  # Built files
│   └── .github/workflows/     # CI/CD workflows
├── 📁 dashboard/              # Private dashboard application
│   ├── server/                # Node.js backend
│   ├── client/                # Frontend application
│   └── database/              # Database schemas and migrations
├── 📁 infrastructure/         # Infrastructure as Code
│   ├── ansible/               # Configuration management
│   ├── kubernetes/            # K8s manifests
│   └── monitoring/            # Monitoring configurations
├── 📁 assets/                 # Images, diagrams, documentation assets
└── 📁 tests/                  # Test suites and validation scripts
```

---

## 🔧 Development

### **Local Development Setup**
```bash
# Install dependencies
npm install

# Set up environment variables
cp .env.example .env
# Edit .env with your configuration

# Start development server
npm run dev

# Run tests
npm test

# Build for production
npm run build
```

### **Contributing Guidelines**
1. **Fork** the repository
2. **Create** a feature branch (`git checkout -b feature/amazing-feature`)
3. **Commit** your changes (`git commit -m 'Add amazing feature'`)
4. **Push** to the branch (`git push origin feature/amazing-feature`)
5. **Open** a Pull Request

### **Code Standards**
- ESLint + Prettier for code formatting
- Conventional Commits for commit messages
- Jest for testing
- JSDoc for documentation

---

## 📊 Monitoring & Observability

### **Key Metrics Tracked**
- **Infrastructure:** CPU, Memory, Disk, Network usage
- **Applications:** Response times, error rates, throughput
- **Security:** Failed login attempts, suspicious activities
- **Business:** User engagement, feature usage

### **Alerting**
- **Critical:** Page immediately for infrastructure failures
- **Warning:** Slack notifications for performance degradation
- **Info:** Email summaries for trend analysis

### **Dashboards**
- **Infrastructure Overview:** System health and capacity
- **Application Performance:** User experience metrics
- **Security Dashboard:** Threat detection and response
- **Business Metrics:** Usage analytics and trends

---

## 🔒 Security

### **Security Measures**
- **Network:** Firewall rules, intrusion detection, VPN access
- **Application:** JWT authentication, input validation, HTTPS only
- **Infrastructure:** Automated updates, configuration hardening
- **Monitoring:** Real-time threat detection and response

### **Compliance**
- Regular security audits
- Automated vulnerability scanning
- Incident response procedures
- Data backup and recovery plans

---

## 📚 Documentation

### **Available Guides**
- [**Architecture Overview**](docs/architecture.md) - System design and components
- [**Setup Guide**](docs/setup-guides/) - Step-by-step installation
- [**API Documentation**](docs/api/) - Backend API reference
- [**Troubleshooting**](docs/troubleshooting.md) - Common issues and solutions
- [**Security Guide**](docs/security.md) - Security best practices

### **External Resources**
- [Raspberry Pi Foundation](https://www.raspberrypi.org/documentation/)
- [Kubernetes Documentation](https://kubernetes.io/docs/)
- [Prometheus Monitoring](https://prometheus.io/docs/)
- [HAProxy Configuration](https://www.haproxy.org/download/2.4/doc/configuration.txt)

---

## 🤝 Support & Community

### **Getting Help**
- 📧 **Email:** [your-email@domain.com](mailto:your-email@domain.com)
- 💬 **Discussions:** [GitHub Discussions](https://github.com/yourusername/homelab-infrastructure/discussions)
- 🐛 **Issues:** [Report Bug](https://github.com/yourusername/homelab-infrastructure/issues/new?template=bug_report.md)
- ✨ **Feature Requests:** [Request Feature](https://github.com/yourusername/homelab-infrastructure/issues/new?template=feature_request.md)

### **Acknowledgments**
- Raspberry Pi Foundation for amazing hardware
- Open source community for incredible tools
- Homelab community for inspiration and guidance

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 🎯 Project Status & Roadmap

**Current Status:** 🟡 **Phase 1 - Foundation Setup**  
**Next Milestone:** 🌐 **Static Portfolio Deployment**  
**Estimated Completion:** 12 weeks from start  
**Infrastructure Value:** $3,300+/year cloud equivalent  

### **Upcoming Features**
- [ ] Home Assistant integration
- [ ] Media server (Plex/Jellyfin)
- [ ] VPN server for remote access
- [ ] Network-attached storage expansion
- [ ] IoT device management

---

<div align="center">

**⭐ Star this repository if you find it helpful!**

![Infrastructure Diagram](./assets/images/infrastructure-overview.png)

*Building enterprise-grade infrastructure, one component at a time* 🚀

</div>
