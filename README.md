# 🧠 WebSphere Application Server (WAS) Learning Guide

## 🌐 What Is WebSphere?
WebSphere is a **platform of enterprise-grade software** developed by IBM to support Java-based applications. It includes multiple products for different business needs:

### Key Products in the WebSphere Suite:
| Product | Description |
|--------|-------------|
| **WebSphere Application Server (WAS)** | Core runtime environment for deploying and managing J2EE applications |
| **WebSphere Portal Server** | Builds and manages web portals |
| **WebSphere Process Server** | Supports business process automation |
| **WebSphere Message Broker (MB)** | Routes and transforms messages between systems |
| **WebSphere MQ** | Messaging middleware for reliable communication between applications |

---

## 🖥️ Server Basics

### Server vs Web Server
| Type | Purpose |
|------|---------|
| **Server** | Executes client requests and runs applications |
| **Web Server** | Serves static and dynamic web content using HTTP/HTTPS |

### Examples of Web Servers:
- Apache
- IIS
- Oracle HTTP Server (OHS)
- IBM HTTP Server (IHS)
- SunOne
- iPlanet

### Tomcat
- Acts as both a **web server** and a **lightweight application server**

---

## 📦 Java EE Packaging Formats

| File Type | Description | Use Case |
|-----------|-------------|----------|
| **.war** (Web Archive) | Contains web modules (JSP, Servlets, HTML) | Web applications (e.g., Gmail, school apps) |
| **.jar** (Java Archive) | Contains EJB modules (Session, Entity, MDB) | Business logic (e.g., banking, IRCTC, LIC) |
| **.ear** (Enterprise Archive) | Combines `.war` and `.jar` | Full enterprise applications |
| **.rar** (Resource Adapter Archive) | Connects to enterprise systems | Integration scenarios |

---

## 🧱 J2EE Components

### JSP (Java Server Pages)
- Java code embedded in HTML
- Executes on the server side

### EJB (Enterprise Java Beans)
- Encapsulates business logic
- Types:
  - **Session Bean**: Stateful or stateless; temporary session data
  - **Entity Bean**: Persistent data storage (e.g., bank, LIC)
  - **Message-Driven Bean**: Handles asynchronous messaging

### JMS (Java Messaging Service)
- Enables messaging between applications (e.g., mobile apps)

### JAAS (Java Authentication and Authorization Service)
- Provides security for authentication and authorization

### JMX (Java Management Extensions)
- Every WAS object is managed via JMX for monitoring and control

---

## 🌍 Client Request Lifecycle

1. **Request Identification**
   - **Static**: Cannot change (e.g., text, PDF, images)
   - **Dynamic**: Interactive content (e.g., JSP, Servlets)

2. **Status Codes**
   - Examples: `404 Not Found`, `500 Internal Server Error`, `502 Bad Gateway`

3. **Deployment**
   - Installing applications on servers
   - Web servers deploy `.war` files

---

## 🚀 Application Server Capabilities

WebSphere Application Server provides:

- J2EE application deployment
- Runtime execution
- Multi-server and multi-application support
- High availability and load balancing
- Robust security

---

## 🏷️ Application Server Market Overview

| Server | Vendor | Latest Version |
|--------|--------|----------------|
| **WebSphere Application Server** | IBM | 8.5 |
| **WebLogic Server** | Oracle | 12c |
| **Apache Tomcat** | Freeware | Varies |
| **JBoss** | Red Hat | 7 |

---

## 🛠️ WAS Administration Essentials

### Prerequisites
- Basic Java knowledge
- Familiarity with Linux (35-hour course recommended)

### Key Concepts
1. **Installation**: Base product setup (no servers initially)
2. **Configuration**: Creating profiles and managing server components
3. **System Management**: Start/stop, backup, restore, sync
4. **Logging**: Log files and rotation policies
5. **Deployment**: `.war`, `.jar`, `.ear` files
6. **JDBC**: Database connectivity
7. **JMS**: Messaging integration
8. **Clusters**:
   - High availability
   - Load balancing
   - Scalability
   - Session management
9. **SSL**: Secure communication
10. **Monitoring**: Tools to track server health
11. **Troubleshooting**: Thread dumps, heap dumps, garbage collection
12. **Maintenance**: Fix packs, upgrades, migrations

---

## 🧩 WAS Terminology

| Term | Description |
|------|-------------|
| **Server** | Execution environment for client requests |
| **Application Server** | Hosts and runs Java applications |
| **Node** | Physical machine hosting application servers |
| **Cell** | Logical grouping of multiple nodes |
| **Profile** | Configuration environment for WAS administration |

### Profile Types:
- **DMGR Profile**: Deployment Manager
- **Application Server Profile**: Hosts applications
- **Custom Profile**: No servers; used for customization
- **Cell Profile**: Combines DMGR and App Server
- **Secure Proxy Profile**: Security gateway
- **Admin Agent Profile**: Manages multiple servers
- **Job Manager Profile**: Manages jobs across environments

---

