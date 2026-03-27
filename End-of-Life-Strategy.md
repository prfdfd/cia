<p align="center">
</p>

<h1 align="center">📅 End-of-Life Strategy — Citizen Intelligence Agency</h1>

<p align="center">
  <strong>🔄 Lifecycle Management and Maintenance Planning</strong><br>
  <em>🎯 Ensuring Stability, Compatibility, and Security Until EOL</em>
</p>

<p align="center">
</p>


---

## Overview

The **CIA Project** will maintain its existing stack, utilizing `javax.*` dependencies and Vaadin 8, without transitioning to Jakarta namespaces. The project will reach EOL when compatibility with the latest JVM requires a Jakarta migration. Below is a structured plan to ensure stability, compatibility, and security until that point.

This strategy should be considered alongside the [Architecture Documentation](ARCHITECTURE.md) to understand the full technical context.

---

## EOL Objective

**Primary Goal**: Maintain the CIA project on its current stack without migrating to Jakarta namespaces, ending support only when essential updates require this shift.

For the current feature set that will be maintained under this strategy, see the [CIA Features page](https://hack23.com/cia-features.html).

## Jetty 10 to Jetty 12 Transition Plan

- **Current Web Server**: The project currently uses **Jetty 10**.
- **EOL for Jetty 10**: Scheduled for **2026** ([endoflife.date](https://endoflife.date/eclipse-jetty)).
- **Potential Move to Jetty 12**: Jetty 12 supports both `javax.servlet` and Jakarta namespaces and has an EOL of **2028**. Migrating to Jetty 12 would allow the CIA project to remain compatible with future JVMs while avoiding an architectural transition to Jakarta.

See [README.md - Deployment Options](README.md#deployment-options) for deployment considerations.

---

## Ongoing Maintenance Strategy

### JVM Compatibility

- **Current Runtime**: Java 26 (Temurin) — production runtime as of 2026
- **Source Compatibility**: Java 21 LTS — source compilation level maintained for stability
- **JVM Monitoring**: Regularly evaluate compatibility with new JVM versions.
- **EOL Trigger**: The project will officially end when updates require Jakarta namespaces for continued compatibility.

#### Java Roadmap & Future Projections

| Java Release | Status | Type | EOL | CIA Platform Impact |
|---|---|---|---|---|
| **Java 21** | ✅ Source Level | LTS | September 2031 | Source compilation target — maintained for stability |
| **Java 22** | 🔵 Compatible | Feature | March 2025 | No changes required |
| **Java 23** | 🔵 Compatible | Feature | March 2025 | No changes required |
| **Java 24** | 🔵 Compatible | Feature | September 2025 | No changes required |
| **Java 25** | 🟡 Compatible | LTS | September 2031 | LTS milestone — previously used as runtime |
| **Java 26** | 🟢 **Current Runtime** | Feature | March 2027 | **Active production runtime** — used in CI/CD and deployments |
| **Java 27** | 🔮 Projected | Feature | March 2028 (est.) | Feature release — compatibility testing planned |
| **Java 28** | 🔮 Projected | Feature | September 2028 (est.) | Feature release |
| **Java 29** | 🔮 Projected | LTS | September 2034 (est.) | Next LTS after 25 — planned runtime upgrade |
| **Java 30** | 🔮 Projected | Feature | March 2029 (est.) | Feature release |
| **Java 31** | 🔮 Projected | Feature | September 2029 (est.) | Feature release |
| **Java 33** | 🔮 Projected | LTS | September 2036 (est.) | Next LTS after 29 — major upgrade candidate if Jakarta migration occurs |

> **Note**: Java feature releases follow a 6-month cadence (March and September). LTS releases occur every 2 years (21, 25, 29, 33…). CIA platform targets the latest available runtime while maintaining Java 21 source compatibility to maximize tooling and library support without requiring a Jakarta namespace migration.

**Runtime Upgrade Strategy**:
- Feature releases: Upgrade runtime within 3 months of release (after CI validation)
- LTS releases: Priority upgrade — validated and deployed within 1 month
- Source level: Remain at Java 21 until Jakarta migration is undertaken

### Dependency Updates

- **Automated Minor and Security Updates**: Dependabot and similar tools will manage minor updates and security patches across core libraries, including:
  - [Spring Security](https://spring.io/projects/spring-security)
  - [Logback](http://logback.qos.ch/)
  - [Bouncy Castle](https://www.bouncycastle.org/)

For security implementation details, see the [Security Architecture](SECURITY_ARCHITECTURE.md).

### Vaadin 8 UI Layer

- **Current UI Strategy**: Continue using **Vaadin 8** to avoid the costs and major structural changes of migrating to Vaadin 10+.
- **Licensing Note**: Vaadin 8 reached EOL for open-source use, so commercial support is available but optional.

For UI component details, see [README.md - Technology Stack](README.md#project-technology-stack).

---

## Final EOL Condition

The CIA project will be designated as EOL and archived in a read-only state when it can no longer function on the latest JVM without adopting Jakarta namespaces.

For the future vision of the platform that may supersede this version, see the [Future Architecture Mindmap](FUTURE_MINDMAP.md).

---

## Project Technology Stack

For a conceptual overview of how these components interact, see the [System Mindmap](MINDMAP.md).

| **Category**                | **Technologies**                                                                                   | **EOL**                     |
|-----------------------------|----------------------------------------------------------------------------------------------------|-----------------------------|
| **Core Framework**          | [Spring Framework 5.x](https://spring.io/projects/spring-framework)                                | **August 31, 2024**             |
| **Security**                | [Spring Security](https://spring.io/projects/spring-security), [Bouncy Castle](https://www.bouncycastle.org/) | Aligns with Spring 5.x |
| **Data Access**             | [Hibernate](https://hibernate.org/), JPA, [PostgreSQL](https://www.postgresql.org/), JDBC          | Hibernate 5.x: Ended; PostgreSQL 18: **Nov 2029** |
| **Transaction Management**  | [Narayana](https://narayana.io/)                                                                   | Active                      |
| **Data Auditing**           | [Javers](https://javers.org/)                                                                      | Active                      |
| **Business Rules Engine**   | [Drools](https://www.drools.org/)                                                                  | Active                      |
| **Messaging**               | [ActiveMQ Artemis](https://activemq.apache.org/components/artemis/), [Spring JMS](https://spring.io/projects/spring-jms) | Active                      |
| **Web/UI Layer**            | [Vaadin 8](https://vaadin.com/docs/latest/guide/vaadin-8/overview), Vaadin Sass Compiler           | Reached EOL; commercial support available |
| **Web Server**              | [Jetty 10.x](https://www.eclipse.org/jetty/) (Potential future move to Jetty 12)                   | Jetty 10 EOL: **2026**; Jetty 12 EOL: **2028** |
| **Monitoring**              | [JavaMelody](https://github.com/javamelody/javamelody), [AWS SDK for CloudWatch](https://aws.amazon.com/cloudwatch/) | Active                      |
| **Testing**                 | [JUnit](https://junit.org/junit5/), [Mockito](https://site.mockito.org/), [Spring Test](https://spring.io/projects/spring-framework), [Selenium WebDriver](https://www.selenium.dev/documentation/) | JUnit 4: Legacy; JUnit 5 & Mockito Active |
| **Utilities**               | [Apache Commons](https://commons.apache.org/), [Google Guava](https://github.com/google/guava), [SLF4J](http://www.slf4j.org/), [Logback](http://logback.qos.ch/), [Jackson](https://github.com/FasterXML/jackson) | Active                      |
| **Build & Dependency Management** | [Maven](https://maven.apache.org/)                                                          | Active                      |

---

## Notes

- **Security Focus**: Prioritize security updates for dependencies in **Spring Security**, **Logback**, and **Bouncy Castle**.
- **Documentation**: See each dependency's documentation for details and licensing options, as summarized on [endoflife.date](https://endoflife.date/).

---

## 📚 Related Documents

### 🏗️ Architecture & Planning
- [🏛️ Architecture](./ARCHITECTURE.md) - Current system architecture
- [🚀 Future Architecture](./FUTURE_ARCHITECTURE.md) - Long-term architectural vision
- [🧠 Future Mindmap](./FUTURE_MINDMAP.md) - Capability expansion plans
- [📋 README](./README.md) - Project overview and quick links

### 🛡️ Security & Compliance
- [🛡️ Security Architecture](./SECURITY_ARCHITECTURE.md) - Current security implementation
- [🎯 Threat Model](./THREAT_MODEL.md) - Lifecycle risk and residual threat alignment

### 🔄 Operations & Workflows
- [🔄 CI/CD Workflows](./WORKFLOWS.md) - Security-hardened CI/CD pipelines
- [🔮 Future Workflows](./FUTURE_WORKFLOWS.md) - Enhanced CI/CD roadmap
- [🚀 CIA Features](https://hack23.com/cia-features.html) - Feature showcase with screenshots
- [📊 Project Documentation](https://hack23.github.io/cia/) - Comprehensive developer resources

---

