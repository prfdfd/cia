# 🔍 Citizen Intelligence Agency

> An independent, volunteer-driven OSINT platform monitoring Swedish political activity

## 🎯 Mission
The Citizen Intelligence Agency is a volunteer-driven, open-source intelligence (OSINT) project that provides comprehensive analysis of political activities in Sweden. Through advanced monitoring of key political figures and institutions, we deliver:

- 📊 Financial performance metrics
- ⚠️ Risk assessment analytics
- 📈 Political trend analysis
- 🏆 Politician ranking system
- 📉 Performance comparisons
- 🔍 Transparency insights

Our initiative remains strictly independent and non-partisan, focused on fostering informed decision-making and enhancing democratic engagement.

## 📊 Quality Metrics

[![Unit Test Coverage](https://img.shields.io/badge/Unit%20Test%20Coverage-JaCoCo%20Results-brightgreen?style=flat-square&logo=java)](https://hack23.github.io/cia/jacoco/)
[![Code Coverage](https://sonarcloud.io/api/project_badges/measure?project=Hack23_cia&metric=coverage)](https://sonarcloud.io/summary/new_code?id=Hack23_cia)
[![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=Hack23_cia&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=Hack23_cia)
[![Lines of Code](https://sonarcloud.io/api/project_badges/measure?project=Hack23_cia&metric=ncloc)](https://sonarcloud.io/summary/new_code?id=Hack23_cia)
[![Technical Debt](https://sonarcloud.io/api/project_badges/measure?project=Hack23_cia&metric=sqale_index)](https://sonarcloud.io/summary/new_code?id=Hack23_cia)
[![Ask DeepWiki](https://deepwiki.com/badge.svg)](https://deepwiki.com/Hack23/cia)


## ✨ Features
Explore our [comprehensive feature set](https://hack23.com/cia-features.html) including:
- 📊 Interactive dashboards
- 🏆 Political scoreboard systems
- 📈 Critical analytics tools
- 🔍 Transparency metrics
- ⚖️ Accountability measures
- 📱 Data-driven insights

For a conceptual view of our system architecture and components, see our [Architecture Documentation](ARCHITECTURE.md) and [System Mindmaps](MINDMAP.md).

## 📚 Data Sources

Our analysis is powered by authoritative Swedish government and international data sources:

| Source | Description |
|--------|-------------|
| 🏛️ [Swedish Parliament Open Data](http://data.riksdagen.se/) | Parliamentary members, committees, and official documents |
| 🗳️ [Swedish Election Authority](http://www.val.se/) | Election data, political parties, and voting results |
| 🌍 [World Bank Open Data](http://data.worldbank.org/) | Global economic indicators and demographic data |
| 💹 [Swedish Financial Management Authority](https://www.esv.se/) | Government finances and economic trends |

## 🏆 Project Status

<div align="center">

[![GitHub Release](https://img.shields.io/github/v/release/Hack23/cia)](https://github.com/Hack23/cia/releases)
[![Ask DeepWiki](https://deepwiki.com/badge.svg)](https://deepwiki.com/Hack23/cia)

[![Verify & Release](https://github.com/Hack23/cia/actions/workflows/release.yml/badge.svg)](https://github.com/Hack23/cia/actions/workflows/release.yml)
[![Verify PR](https://github.com/Hack23/cia/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/Hack23/cia/actions/workflows/codeql-analysis.yml)
[![Lines of Code](https://sonarcloud.io/api/project_badges/measure?project=Hack23_cia&metric=ncloc)](https://sonarcloud.io/summary/new_code?id=Hack23_cia)

[![Average time to resolve an issue](https://isitmaintained.com/badge/resolution/Hack23/cia.svg)](https://isitmaintained.com/project/Hack23/cia "Average time to resolve an issue")
[![Percentage of issues still open](https://isitmaintained.com/badge/open/Hack23/cia.svg)](https://isitmaintained.com/project/Hack23/cia "Percentage of issues still open")
[![CLA assistant](https://cla-assistant.io/readme/badge/Hack23/cia)](https://cla-assistant.io/Hack23/cia)

</div>

## 🚀 Runtime Environment

<div align="center">

| JDK Version | Status | Release Info |
|-------------|--------|--------------|
| ![JDK-21](https://img.shields.io/badge/JDK-21-brightgreen.svg) | Source Level | LTS - Source Compatibility |
| ![JDK-22](https://img.shields.io/badge/JDK-22-orange.svg) | Compatible | Feature Release |
| ![JDK-23](https://img.shields.io/badge/JDK-23-orange.svg) | Compatible | Feature Release |
| ![JDK-24](https://img.shields.io/badge/JDK-24-orange.svg) | Compatible | Feature Release |
| ![JDK-25](https://img.shields.io/badge/JDK-25-brightgreen.svg) | Compatible (LTS) | LTS Release — Previous Production Runtime |
| ![JDK-26](https://img.shields.io/badge/JDK-26-brightgreen.svg) | **Current Runtime** | Feature Release — Active Production Runtime |

**Build Configuration:** Source Java 21, Target Java 21, Runtime Java 26

</div>

For details on our technology lifecycle management, see the [End-of-Life Strategy](End-of-Life-Strategy.md).

## 🛠️ Development Environment Requirements

<div align="center">

| Component | Version | Purpose | Reference |
|-----------|---------|---------|-----------|
| **Java JDK** | 26 (Temurin) | Runtime environment | [Setup Java](https://adoptium.net/) |
| **Java Source** | 21 | Source compatibility | Maven compiler configuration |
| **Maven** | 3.9.14+ | Build automation | [Maven Install](https://maven.apache.org/install.html) |
| **Node.js** | 24+ | Playwright testing | [Node.js](https://nodejs.org/) |
| **PostgreSQL** | 16+ | Database (optional for full integration testing) | [PostgreSQL](https://www.postgresql.org/) |

</div>

**Quick Start:**
```bash
# Build the project (skipping tests)
mvn clean install -DskipTests

# Build with tests
mvn clean install

# Run specific module
cd citizen-intelligence-agency
mvn spring-boot:run
```

## 📚 Architecture Documentation Map

<div class="documentation-map">

| Document                                            | Focus           | Description                               | Documentation Link                                                              |
| --------------------------------------------------- | --------------- | ----------------------------------------- | ------------------------------------------------------------------------------- |
| **[Architecture](ARCHITECTURE.md)**                 | 🏛️ Architecture | C4 model showing current system structure | [View Source](https://github.com/Hack23/cia/blob/master/ARCHITECTURE.md)         |
| **[Future Architecture](FUTURE_ARCHITECTURE.md)**   | 🏛️ Architecture | C4 model showing future system structure | [View Source](https://github.com/Hack23/cia/blob/master/FUTURE_ARCHITECTURE.md)         |
| **[Security Architecture](SECURITY_ARCHITECTURE.md)** | 🔐 Security     | Security architecture                     | [View Source](https://github.com/Hack23/cia/blob/master/SECURITY_ARCHITECTURE.md)         |
| **[Future Security Architecture](FUTURE_SECURITY_ARCHITECTURE.md)** | 🔐 Security     | Future Security architecture  | [View Source](https://github.com/Hack23/cia/blob/master/FUTURE_SECURITY_ARCHITECTURE.md)         |
| **[Mindmaps](MINDMAP.md)**                          | 🧠 Concept      | Current system component relationships    | [View Source](https://github.com/Hack23/cia/blob/master/MINDMAP.md)             |
| **[Future Mindmaps](FUTURE_MINDMAP.md)**            | 🧠 Concept      | Future capability evolution               | [View Source](https://github.com/Hack23/cia/blob/master/FUTURE_MINDMAP.md)      |
| **[SWOT Analysis](SWOT.md)**                        | 💼 Business     | Current strategic assessment              | [View Source](https://github.com/Hack23/cia/blob/master/SWOT.md)                |
| **[Future SWOT Analysis](FUTURE_SWOT.md)**          | 💼 Business     | Future strategic opportunities            | [View Source](https://github.com/Hack23/cia/blob/master/FUTURE_SWOT.md)         |
| **[Data Model](DATA_MODEL.md)**                     | 📊 Data         | Current data structures and relationships | [View Source](https://github.com/Hack23/cia/blob/master/DATA_MODEL.md)          |
| **[Future Data Model](FUTURE_DATA_MODEL.md)**       | 📊 Data         | Enhanced political data architecture      | [View Source](https://github.com/Hack23/cia/blob/master/FUTURE_DATA_MODEL.md)   |
| **[Flowcharts](FLOWCHART.md)**                      | 🔄 Process      | Current data processing workflows         | [View Source](https://github.com/Hack23/cia/blob/master/FLOWCHART.md)           |
| **[Future Flowcharts](FUTURE_FLOWCHART.md)**        | 🔄 Process      | Enhanced AI-driven workflows              | [View Source](https://github.com/Hack23/cia/blob/master/FUTURE_FLOWCHART.md)    |
| **[State Diagrams](STATEDIAGRAM.md)**               | 🔄 Behavior     | Current system state transitions          | [View Source](https://github.com/Hack23/cia/blob/master/STATEDIAGRAM.md)        |
| **[Future State Diagrams](FUTURE_STATEDIAGRAM.md)** | 🔄 Behavior     | Enhanced adaptive state transitions       | [View Source](https://github.com/Hack23/cia/blob/master/FUTURE_STATEDIAGRAM.md) |
| **[CI/CD Workflows](WORKFLOWS.md)**                 | 🔧 DevOps       | Current automation processes              | [View Source](https://github.com/Hack23/cia/blob/master/WORKFLOWS.md)           |
| **[Future Workflows](FUTURE_WORKFLOWS.md)**         | 🔧 DevOps       | Enhanced CI/CD with ML                    | [View Source](https://github.com/Hack23/cia/blob/master/FUTURE_WORKFLOWS.md)    |
| **[End-of-Life Strategy](End-of-Life-Strategy.md)** | 📅 Lifecycle    | Maintenance and EOL planning              | [View Source](https://github.com/Hack23/cia/blob/master/End-of-Life-Strategy.md) |
| **[CIA Features](https://hack23.com/cia-features.html)** | 🚀 Features | Platform features overview                | [View on hack23.com](https://hack23.com/cia-features.html)                     |
| **[Threat Model](THREAT_MODEL.md)**                 | 🛡️ Security     | STRIDE / MITRE risk analysis              | [View Source](https://github.com/Hack23/cia/blob/master/THREAT_MODEL.md)        |
| **[Unit Test Plan](UnitTestPlan.md)**               | 🧪 Testing      | Comprehensive testing strategy & coverage | [View Source](https://github.com/Hack23/cia/blob/master/UnitTestPlan.md)        |

</div>

## 🔍 Intelligence & Analytics Documentation

<div class="intelligence-documentation">

The CIA platform provides comprehensive intelligence operations (INTOP) and open-source intelligence (OSINT) capabilities. Our intelligence documentation tracks the evolution of analytical frameworks, risk assessment rules, and database views that power political intelligence products.

### 📋 Intelligence Changelog

Unified tracking of intelligence evolution across all capabilities:

| Document | Focus | Description | Documentation Link |
|----------|-------|-------------|-------------------|
| **[Intelligence Evolution Changelog](CHANGELOG_INTELLIGENCE.md)** | 🎯 Unified | Comprehensive tracking of intelligence capabilities, database views, risk rules, and analytical frameworks | [View Source](https://github.com/Hack23/cia/blob/master/CHANGELOG_INTELLIGENCE.md) |

**Historical Changelogs** (Archived): [Intelligence Analysis](docs/archive/CHANGELOG_INTELLIGENCE_ANALYSIS.md), [Database Views](docs/archive/CHANGELOG_DATABASE_VIEWS.md), [Risk Rules](docs/archive/CHANGELOG_RISK_RULES.md)

### 📚 Core Intelligence Documentation

Comprehensive documentation of analytical capabilities and methodologies:

| Document | Focus | Description | Documentation Link |
|----------|-------|-------------|-------------------|
| **[Data Analysis - INTOP OSINT](DATA_ANALYSIS_INTOP_OSINT.md)** | 🎯 Frameworks | 6 analysis frameworks (Temporal, Comparative, Pattern Recognition, Predictive, Network, Decision) | [View Source](https://github.com/Hack23/cia/blob/master/DATA_ANALYSIS_INTOP_OSINT.md) |
| **[Risk Rules Documentation](RISK_RULES_INTOP_OSINT.md)** | 🔴 Risk Rules | 50 behavioral detection rules (24 politician, 10 party, 4 committee, 4 ministry, 5 decision, 3 other) | [View Source](https://github.com/Hack23/cia/blob/master/RISK_RULES_INTOP_OSINT.md) |
| **[Database View Intelligence Catalog](DATABASE_VIEW_INTELLIGENCE_CATALOG.md)** | 🗄️ Views | Complete catalog of 85 database views (57 regular + 28 materialized) | [View Source](https://github.com/Hack23/cia/blob/master/DATABASE_VIEW_INTELLIGENCE_CATALOG.md) |
| **[Data Quality Monitoring Dashboard](DATA_QUALITY_MONITORING_DASHBOARD.md)** | 📊 Quality | Unified data quality monitoring with OSINT, database health, and view validation metrics | [View Source](https://github.com/Hack23/cia/blob/master/DATA_QUALITY_MONITORING_DASHBOARD.md) |
| **[Intelligence Data Flow Map](INTELLIGENCE_DATA_FLOW.md)** | 🗺️ Pipeline | Data pipeline mappings and framework-to-view relationships | [View Source](https://github.com/Hack23/cia/blob/master/INTELLIGENCE_DATA_FLOW.md) |
| **[Liquibase Intelligence Analysis](LIQUIBASE_CHANGELOG_INTELLIGENCE_ANALYSIS.md)** | 🗄️ Schema | Database schema evolution from intelligence perspective | [View Source](https://github.com/Hack23/cia/blob/master/LIQUIBASE_CHANGELOG_INTELLIGENCE_ANALYSIS.md) |

### 🛠️ Intelligence Automation

| Tool | Purpose | Location |
|------|---------|----------|
| **Intelligence Changelog Generator** | Automated detection of view changes, risk rule updates, and framework enhancements | [Script](.github/scripts/generate-intelligence-changelog.sh) |
| **GitHub Actions Workflow** | Automated changelog generation on demand | [Workflow](.github/workflows/generate-intelligence-changelog.yml) |

**Usage:**
```bash
# Generate intelligence changelog from recent changes
.github/scripts/generate-intelligence-changelog.sh

# Compare specific commits
.github/scripts/generate-intelligence-changelog.sh <prev_commit> <current_commit>
```

### 📊 Intelligence Metrics (v1.36.0)

| Category | Count | Description |
|----------|-------|-------------|
| **Analysis Frameworks** | 6 | Temporal, Comparative, Pattern Recognition, Predictive, Network, Decision Intelligence |
| **Risk Rules** | 50 | 24 politician + 10 party + 4 committee + 4 ministry + 5 decision + 3 other |
| **Database Views** | 85 | 57 regular views + 28 materialized views |
| **OSINT Data Sources** | 4 | Riksdagen API, Election Authority, World Bank, Financial Authority |
| **Intelligence Products** | 10+ | Scorecards, Coalition Analysis, Risk Assessments, Trend Reports, Decision Tracking |

### 📖 Documentation Navigation Guide

Navigate intelligence documentation efficiently based on your role:

<table>
<tr>
<td width="50%">

#### 📊 For Data Analysts
**Goal:** Find views and analytical capabilities

1. **Start**: [Data Analysis Frameworks](DATA_ANALYSIS_INTOP_OSINT.md) - Explore 6 analytical frameworks
2. **Then**: [Database View Intelligence Catalog](DATABASE_VIEW_INTELLIGENCE_CATALOG.md) - Discover 84 database views
3. **Reference**: [Intelligence Data Flow Map](INTELLIGENCE_DATA_FLOW.md) - Understand data pipelines

**Key Use Cases:**
- Finding views for specific analysis types (temporal, comparative, pattern recognition)
- Understanding view relationships and dependencies
- Accessing sample queries and usage patterns

</td>
<td width="50%">

#### 🕵️ For Intelligence Operatives
**Goal:** Understand complete intelligence pipeline

1. **Start**: [Intelligence Data Flow Map](INTELLIGENCE_DATA_FLOW.md) - Complete data pipeline overview
2. **Then**: [Data Analysis Frameworks](DATA_ANALYSIS_INTOP_OSINT.md) - OSINT methodologies and frameworks
3. **Deep Dive**: [Risk Rules Documentation](RISK_RULES_INTOP_OSINT.md) - 50 behavioral detection rules

**Key Use Cases:**
- Understanding OSINT collection methods
- Analyzing behavioral patterns and anomalies
- Generating intelligence products and assessments

</td>
</tr>
<tr>
<td width="50%">

#### 🗄️ For Database Administrators
**Goal:** Maintain schema and optimize performance

1. **Start**: [Schema Maintenance Guide](service.data.impl/README-SCHEMA-MAINTENANCE.md) - Database maintenance procedures
2. **Then**: [Data Quality Monitoring Dashboard](DATA_QUALITY_MONITORING_DASHBOARD.md) - Monitor database health and quality metrics
3. **Reference**: [Database View Intelligence Catalog](DATABASE_VIEW_INTELLIGENCE_CATALOG.md) - View documentation and optimization
4. **Track Changes**: [Intelligence Evolution Changelog](CHANGELOG_INTELLIGENCE.md) - Schema evolution history

**Key Use Cases:**
- Monitoring database health and data quality metrics
- Refreshing materialized views
- Running health checks and validation
- Understanding view dependencies and usage patterns
- Performance tuning and index optimization

</td>
<td width="50%">

#### 📈 For Product Managers
**Goal:** Understand capabilities and product features

1. **Start**: [Data Analysis Frameworks](DATA_ANALYSIS_INTOP_OSINT.md) - Analytical capabilities overview
3. **Explore**: [Database View Intelligence Catalog](DATABASE_VIEW_INTELLIGENCE_CATALOG.md) - Data products inventory

> _Note: See [Related Documentation in Intelligence Data Flow](INTELLIGENCE_DATA_FLOW.md#-related-documentation) for complete document cross-references._

**Key Use Cases:**
- Understanding product capabilities and intelligence products
- Identifying feature gaps and opportunities
- Planning roadmap and prioritizing enhancements

</td>
</tr>
</table>

**Quick Links:**
- 🗺️ [Intelligence Data Flow Map](INTELLIGENCE_DATA_FLOW.md) - Central navigation hub
- 📜 [Intelligence Evolution Changelog](CHANGELOG_INTELLIGENCE.md) - Capability tracking over time
- 🔍 [OSINT Data Sources](#-data-sources) - External API integrations
- 📊 [Intelligence Metrics](#-intelligence-metrics-v1360) - Current capability counts

</div>

## 🔒 Reporting Security Issues

Please follow the instructions in our [SECURITY.md](https://github.com/Hack23/cia/blob/master/SECURITY.md) file for reporting security issues.

## 🔧 Project Technology Stack

<div align="center">

### 📚 Core Technology Stack

This document provides a high-level overview of the key technologies used within the **Citizen Intelligence Agency (CIA)** project. Each technology plays a vital role in supporting CIA’s goals for data analysis, security, and scalability within the political intelligence domain.

| **Category**              | **Technologies**                                                                                                                                                   |
|---------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Core Framework**        | [Spring Framework](https://spring.io/projects/spring-framework)                                                                                                   |
| **Security**              | [Spring Security](https://spring.io/projects/spring-security), [Bouncy Castle](https://www.bouncycastle.org/)                                                     |
| **Data Access**           | [Hibernate](https://hibernate.org/orm/), [JPA](https://jakarta.ee/specifications/persistence/), [PostgreSQL](https://www.postgresql.org/), [JDBC](https://docs.oracle.com/javase/tutorial/jdbc/overview/index.html) |
| **Transaction Management**| [Narayana](https://narayana.io/) (Integrated with Spring `JpaTransactionManager`)                                           |
| **Data Auditing**         | [Javers](https://javers.org/)                                                                                                                                     |
| **Business Rules Engine** | [Drools](https://www.drools.org/)                                                                                                                                 |
| **Messaging**             | [ActiveMQ Artemis](https://activemq.apache.org/components/artemis/), [Spring JMS](https://spring.io/projects/spring-framework)                                    |
| **Web/UI Layer**          | [Vaadin](https://vaadin.com/), [Vaadin Sass Compiler](http://vaadin.com/), [Vaadin Themes](https://vaadin.com/)                                                  |
| **Monitoring**            | [JavaMelody](https://github.com/javamelody/javamelody), [AWS SDK for CloudWatch](https://aws.amazon.com/cloudwatch/)                                              |
| **Testing**               | [JUnit](https://junit.org/), [Mockito](https://site.mockito.org/), [Spring Test](https://docs.spring.io/spring-framework/docs/current/reference/html/testing.html), [Selenium WebDriver](https://www.selenium.dev/documentation/en/webdriver/) |
| **Utilities**             | [Apache Commons](https://commons.apache.org/), [Google Guava](https://guava.dev/), [SLF4J](http://www.slf4j.org/), [Logback](https://logback.qos.ch/), [Jackson](https://github.com/FasterXML/jackson) |
| **Build & Dependency Management** | [Maven](https://maven.apache.org/)                                                                                                                           |

</div>

## 🚀 Deployment Options

### AWS CloudFormation Deployment

The Citizen Intelligence Agency can be deployed on AWS using our provided CloudFormation template:

1. Download the [CloudFormation stack file](cia-dist-cloudformation/src/main/resources/cia-dist-cloudformation.json)
2. Create a new stack in the AWS CloudFormation console
3. Upload the template file and configure parameters
4. Acknowledge IAM resource creation and launch the stack
5. Access the application via the URL in the stack outputs

#### CloudFormation Stack Diagram
![Cloudformation stack Diagram](cia-dist-cloudformation/src/main/resources/cia-dist-cloudformation.png)

### Debian/Ubuntu Installation

For local or self-hosted deployment on Debian/Ubuntu 24.04+:

1. Add the PostgreSQL PGDG repository (required for PostgreSQL 18 on Ubuntu 24.04):
   ```bash
   sudo install -d /usr/share/postgresql-common/pgdg
   sudo curl -o /usr/share/postgresql-common/pgdg/apt.postgresql.org.asc --fail https://www.postgresql.org/media/keys/ACCC4CF8.asc
   echo "deb [signed-by=/usr/share/postgresql-common/pgdg/apt.postgresql.org.asc] https://apt.postgresql.org/pub/repos/apt $(lsb_release -cs)-pgdg main" | sudo tee /etc/apt/sources.list.d/pgdg.list
   sudo apt-get update
   ```

2. Install prerequisites:
   ```bash
   sudo apt-get install openjdk-21-jdk postgresql-18 postgresql-contrib-18 postgresql-18-pgaudit postgresql-18-pgvector
   ```

3. Configure PostgreSQL as detailed below.

## PostgreSQL 18 Configuration Guide

A step-by-step guide to configure PostgreSQL 18 with SSL, prepared transactions, and required extensions.

### 1. Enable Prepared Transactions and Required Extensions

1. **Edit** `/etc/postgresql/18/main/postgresql.conf` and add or update the following lines:
   ```ini
   max_prepared_transactions = 100
   shared_preload_libraries = 'pg_stat_statements, pgaudit, pgcrypto'
   pgaudit.log = ddl
   pg_stat_statements.track = all
   pg_stat_statements.max = 10000
   ```
2. **Save and close** the file.

### 2. Update `pg_hba.conf` for IPv6 Loopback Access

1. **Edit** `/etc/postgresql/18/main/pg_hba.conf` and add the following line:
   ```ini
   host all all ::1/128 md5
   ```
2. **Save and close** the file.

### 3. Generate SSL Certificates and Keys

1. Generate a secure random passphrase:
   ```bash
   openssl rand -base64 48 > passphrase.txt
   ```

2. Create a passphrase-protected private key:
   ```bash
   openssl genrsa -des3 -passout file:passphrase.txt -out server.pass.key 2048
   ```

3. Remove the passphrase protection from the private key:
   ```bash
   openssl rsa -passin file:passphrase.txt -in server.pass.key -out server.key
   rm server.pass.key
   ```

4. Create a Certificate Signing Request (CSR):
   ```bash
   openssl req -new -key server.key -out server.csr \
       -subj "/C=UK/ST=Postgresqll/L=Docker/O=Hack23/OU=demo/CN=127.0.0.1"
   ```

5. Self-sign the certificate (valid for 10 years / 3650 days):
   ```bash
   openssl x509 -req -days 3650 -in server.csr -signkey server.key -out server.crt
   ```

6. Clean up temporary files:
   ```bash
   rm passphrase.txt
   rm server.csr
   ```

### 4. Deploy the SSL Certificate and Key for PostgreSQL

1. Copy the new certificate and key into the PostgreSQL data directory:
   ```bash
   cp server.crt /var/lib/postgresql/18/main/server.crt
   cp server.key /var/lib/postgresql/18/main/server.key
   rm server.key
   ```

2. Secure the certificate and key:
   ```bash
   chmod 600 /var/lib/postgresql/18/main/server.key
   chmod 644 /var/lib/postgresql/18/main/server.crt
   chown -R postgres:postgres /var/lib/postgresql/18/main/
   ```

3. Enable SSL in PostgreSQL by adding the following lines to
   `/etc/postgresql/18/main/postgresql.conf`:
   ```bash
   echo "ssl_cert_file = '/var/lib/postgresql/18/main/server.crt'" \
       >> /etc/postgresql/18/main/postgresql.conf
   echo "ssl_key_file = '/var/lib/postgresql/18/main/server.key'" \
       >> /etc/postgresql/18/main/postgresql.conf
   ```

### 5. Provide SSL Certificate to the `cia` User

1. Create a `.postgresql` directory for the `cia` user:
   ```bash
   mkdir -p /opt/cia/.postgresql
   ```

2. Copy the server certificate into this directory:
   ```bash
   cp server.crt /opt/cia/.postgresql/root.crt
   chmod 700 /opt/cia/.postgresql/root.crt
   chown -R cia:cia /opt/cia/.postgresql/root.crt
   ```

3. Remove the server certificate from the current directory (if desired):
   ```bash
   rm server.crt
   ```

### 6. Performance Tuning (Recommended)

For optimal performance with the CIA platform's 85+ views and 93 tables, add the following settings to `/etc/postgresql/18/main/postgresql.conf`. Values should be adjusted based on your server's available RAM.

#### Memory Settings

Configure memory settings proportionally to your system RAM:

| Setting                  | 4GB RAM | 8GB RAM | 16GB+ RAM (Production) |
|--------------------------|---------|---------|------------------------|
| `shared_buffers`         | 1GB     | 2GB     | 4GB                    |
| `effective_cache_size`   | 3GB     | 6GB     | 12GB                   |
| `maintenance_work_mem`   | 256MB   | 512MB   | 1GB                    |
| `work_mem`               | 16MB    | 32MB    | 50MB                   |

Apply settings using SQL commands (use values from the table above for your RAM configuration):

```sql
-- Example for 8GB RAM server - adjust values from the table above for your configuration
-- shared_buffers: ~25% of RAM
-- effective_cache_size: ~75% of RAM
-- maintenance_work_mem: For VACUUM, CREATE INDEX operations
-- work_mem: Per-operation memory for sorts, joins

ALTER SYSTEM SET shared_buffers = '2GB';
ALTER SYSTEM SET effective_cache_size = '6GB';
ALTER SYSTEM SET maintenance_work_mem = '512MB';
ALTER SYSTEM SET work_mem = '32MB';
```

#### Checkpoint Settings

Configure checkpoint settings for optimal write performance:

```sql
ALTER SYSTEM SET checkpoint_completion_target = 0.9;
ALTER SYSTEM SET wal_buffers = '16MB';
ALTER SYSTEM SET max_wal_size = '4GB';
ALTER SYSTEM SET min_wal_size = '1GB';
```

#### Query Planning Optimizations

For SSD storage (recommended), optimize query planning:

```sql
ALTER SYSTEM SET random_page_cost = 1.1;        -- For SSD storage
ALTER SYSTEM SET effective_io_concurrency = 200; -- For SSD storage
```

#### Connection Settings

Configure connection limits:

```sql
ALTER SYSTEM SET max_connections = 200;
```

#### Apply Settings

After making changes, apply them:

```bash
# Reload configuration (for settings that don't require restart)
sudo -u postgres psql -c "SELECT pg_reload_conf();"

# For settings requiring restart (shared_buffers, max_connections):
sudo systemctl restart postgresql
```

#### Verify Settings

Confirm settings are applied:

```sql
-- Check current settings
SHOW shared_buffers;
SHOW effective_cache_size;
SHOW work_mem;
SHOW maintenance_work_mem;
SHOW checkpoint_completion_target;
SHOW random_page_cost;
SHOW max_connections;
```

> **📚 Note:** For detailed performance tuning guidelines, database health monitoring, and advanced configuration options, see [service.data.impl/README-SCHEMA-MAINTENANCE.md](service.data.impl/README-SCHEMA-MAINTENANCE.md).

### Final Steps

1. **Restart PostgreSQL** to apply all changes:
   ```bash
   systemctl restart postgresql
   ```

2. Verify that PostgreSQL is running with SSL by checking the logs or using an SSL-enabled client.

3. Confirm that prepared transactions and required extensions are enabled:
   ```sql
   SHOW max_prepared_transactions;
   \dx
   ```

4. Confirm the new IPv6 entry in `pg_hba.conf` is functioning as expected by connecting via `psql` over `::1`.

## Database Setup

Create an empty database:

Below instructions set the default username/password and database name used for development. We recommend using custom credentials and updating the configuration at `/opt/cia/webapps/cia/WEB-INF/database.properties` to define your own username/password and database name.

```bash
$ sudo su - postgres
$ psql
postgres=# CREATE USER eris WITH password 'discord';
postgres=# CREATE DATABASE cia_dev;
postgres=# GRANT ALL PRIVILEGES ON DATABASE cia_dev to eris;
```

## Install CIA Debian Package

1. Download the CIA Debian package:
   ```bash
   wget https://github.com/Hack23/cia/releases/download/2025.1.2/cia-dist-deb-2025.1.2.all.deb
   ```

2. Install the Debian package:
   ```bash
   sudo dpkg -i cia-dist-deb-2025.1.2.all.deb
   ```

3. Access the server at [https://localhost:28443/cia/](https://localhost:28443/cia/).

## macOS (Apple Silicon / M1) Development Setup

### Prerequisites

Install the required tools via [Homebrew](https://brew.sh/):

```bash
# Install Java 21 (source level) - arm64 native
brew install --cask temurin@21

# Install Maven
brew install maven

# Install PostgreSQL 18
brew install postgresql@18
```

### Start PostgreSQL

```bash
brew services start postgresql@18
```

### Configure PostgreSQL

1. Find your PostgreSQL config directory:
   ```bash
   psql -U $(whoami) -d postgres -c "SHOW config_file;"
   ```

2. Edit `postgresql.conf` and add:
   ```ini
   max_prepared_transactions = 100
   shared_preload_libraries = 'pg_stat_statements'
   ```

3. Restart PostgreSQL:
   ```bash
   brew services restart postgresql@18
   ```

### Create the Database

```bash
psql -U $(whoami) -d postgres -c "CREATE USER eris WITH password 'discord';"
psql -U $(whoami) -d postgres -c "CREATE DATABASE cia_dev;"
psql -U $(whoami) -d postgres -c "GRANT ALL PRIVILEGES ON DATABASE cia_dev to eris;"
```

### Build and Run

```bash
# Clone the repository
git clone https://github.com/Hack23/cia.git
cd cia

# Build (skip tests for faster first build)
mvn clean install -DskipTests

# Build with tests
mvn clean install

# Run the application
cd citizen-intelligence-agency
mvn spring-boot:run
```

Access the application at [https://localhost:28443/cia/](https://localhost:28443/cia/).

> **Note:** The project source level is Java 21. The production runtime targets Java 26, but Java 21 is sufficient for local development on Apple Silicon.

## 📊 Political Dashboards

- **English**: Our [dashboard](https://github.com/Hack23/cia/blob/master/dashboard.md) provides comprehensive analytics on Swedish political figures and institutions.

- **Swedish**: Vår [dashboard](https://github.com/Hack23/cia/blob/master/dashboard_sv.md) erbjuder en detaljerad översikt över politiska figurer och olika departement i Sverige.

## 🤖 AI and Data Visualization

This project is powered by advanced AI technologies for data processing and analysis. We integrate data from various open sources and visualize findings through modern data visualization tools.

For our future vision incorporating more advanced AI capabilities, see our [Future Architecture Vision](FUTURE_MINDMAP.md).



## 📚 Related Documents

### 🏛️ Architecture & Design
- [🏗️ Architecture Documentation](ARCHITECTURE.md) - C4 model system architecture
- [🧠 System Mindmaps](MINDMAP.md) - Conceptual overview and component relationships
- [🚀 Future Architecture Vision](FUTURE_MINDMAP.md) - AI-enhanced capabilities roadmap
- [📊 Data Model](DATA_MODEL.md) - Database schema and entity relationships
- [🗄️ Entity Model Documentation](https://hack23.github.io/cia/service.data.impl/hbm2doc/entities/index.html) - Detailed database entity reference
- [📋 API Documentation](https://hack23.github.io/cia/apidocs/index.html) - Complete API reference
- [📦 Package Dependencies](https://hack23.github.io/cia/apidocs/package-dependencies.svg) - Visual code package structure

### 🛡️ Security & Compliance
- [🔐 Security Architecture](SECURITY_ARCHITECTURE.md) - Defense-in-depth security implementation
- [🚀 Future Security Architecture](FUTURE_SECURITY_ARCHITECTURE.md) - Advanced security capabilities roadmap
- [🎯 Threat Model](THREAT_MODEL.md) - STRIDE/MITRE ATT&CK threat analysis
- [🔒 Security Policy](SECURITY.md) - Vulnerability disclosure and security reporting

### 🔄 Operations & Development
- [⚡ Workflows](WORKFLOWS.md) - CI/CD pipelines and DevSecOps automation
- [📅 End-of-Life Strategy](End-of-Life-Strategy.md) - Technology maintenance and lifecycle planning
- [🧪 Unit Test Plan](UnitTestPlan.md) - Testing strategy and coverage requirements
- [🌐 E2E Test Plan](E2ETestPlan.md) - End-to-end testing documentation
- [🤝 Contributing Guidelines](CONTRIBUTING.md) - Development contribution guide
- [📜 Code of Conduct](CODE_OF_CONDUCT.md) - Community standards and expectations

### 🎨 Features & Dashboards
- [✨ CIA Features Showcase](https://hack23.com/cia-features.html) - Comprehensive feature demonstrations
- [📊 Political Dashboard (English)](dashboard.md) - Swedish political analytics
- [📊 Politisk Dashboard (Svenska)](dashboard_sv.md) - Svensk politisk analys

