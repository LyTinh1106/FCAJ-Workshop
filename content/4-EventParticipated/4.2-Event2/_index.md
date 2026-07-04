---
title: "Event Meet up  06-06-2026"
date: 2026-06-06
weight: 2
chapter: false
pre: " <b> 4.2. </b> "
---

### Event Objectives

*   Share practical experiences and valuable lessons learned during learning, self-study, and cloud/AI technology project development.
*   Exchange in-depth knowledge of containerization technology, real-time connection programming, intrusion detection systems, and modern GraphRAG solutions.
*   Promote effective teamwork practices, cultivate system design thinking, and establish a clear roadmap for personal growth from entry-level to senior positions.

### Speakers

*   **Nguyen Quoc Bao** - Godot Client & AWS WebSockets.
*   **Bao Huynh** - Containerization Technology with Docker.
*   **Viet Phat** - GraphRAG Solution with Bedrock & Neptune.
*   **Le Hoang Gia Dai** - Machine Learning-based NIDS.
*   **Truong Huy Phuoc** - The Art of Effective Teamwork.
*   **Tran Trung Vinh** - Journey from IT Helpdesk to Senior Sysadmin.

---

## Event Highlights

### 1. Connecting Godot Client with AWS WebSockets for Multiplayer Games (Nguyen Quoc Bao)
*   **Serverless Bi-directional Architecture**: Harnesses AWS API Gateway WebSockets to maintain persistent connections with minimal latency, backed by AWS Lambda for game logic and Amazon DynamoDB for real-time game state tracking.
*   **Godot Engine Integration**: Implements the `WebSocketPeer` class and optimizes the `_process` loop to guarantee instant data packet delivery and real-time multiplayer synchronization.
*   **Practical Mitigations**: Shares methods to control DynamoDB query costs and implement garbage collection for "stale" connections in database records to prevent resource leakage.

### 2. Containerization Technology with Docker (Bao Huynh)
*   **Comprehensive Packaging Solution**: Bundles applications with all their libraries, configurations, and dependencies into a single Docker Image to eradicate the "it works on my machine" issue.
*   **Resource Optimization**: Shares the host operating system kernel instead of running a full guest OS (like VMs), allowing containers to boot in seconds and consume minimal CPU and memory.
*   **Accelerated CI/CD & Microservices**: Empowers rapid development and deployment automation through three key components: Dockerfiles (build recipes), Docker Images (read-only templates), and Docker Containers (active runtime instances).

### 3. GraphRAG Solution with Amazon Bedrock and Neptune (Viet Phat)
*   **Enhancing Traditional RAG**: Constructs Knowledge Graphs to allow LLMs to perform complex multi-hop reasoning queries and map deep entity relationships.
*   **Dual Deployment Paths**:
     *   **Fully Managed**: Employs Amazon Bedrock Knowledge Bases integrated with Neptune Analytics for fast deployment.
     *   **Custom**: Employs LlamaIndex to build customized ETL pipelines, allowing direct Cypher query executions on Amazon Neptune for maximum flexibility.

### 4. Machine Learning-based Network Intrusion Detection System (Le Hoang Gia Dai)
*   **Hybrid Security Approach**: Integrates rule-based AWS WAF with Machine Learning algorithms to identify anomalous behaviors and Zero-day attacks that traditional firewalls overlook.
*   **Model Training Process**: Leverages the CSE-CIC-IDS2018 dataset to train ML models to accurately classify attacks like Botnets, DoS, DDoS, and Brute Force.
*   **Detection Optimization**: Uses advanced data balancing techniques to enhance model sensitivity to minority attack classes and interfaces with a real-time visualization Dashboard.

### 5. The Art of Effective Teamwork (Truong Huy Phuoc)
*   **4 Golden Collaboration Rules**: Focuses on setting clear goals, aligning task assignments with team members' strengths, maintaining transparent communication, and ensuring strong personal accountability.
*   **Synergized Group Efficiency**: Promotes the "many hands make light work" philosophy to share tasks effectively, maximize productivity, and dissolve communication silos.
*   **Digital Workspaces**: Recommends platforms like Trello for visual scheduling, Slack & Discord for immediate collaboration, and Google Workspace for co-authoring documents.

### 6. Journey from IT Helpdesk to Senior Sysadmin (Tran Trung Vinh)
*   **Empirical Growth & Self-study**: Portrays a real career progression from basic desktop support (Helpdesk) to senior systems administrator, expanding subsequently into Cloud and DevOps.
*   **Mindset Transformation**: Shifts focus from fixing isolated issues to understanding systemic design, urging juniors to master Linux, Networking, and engage in continuous lab testing.
*   **Ultimate Sysadmin Rule**: Stresses the fundamental rule of production safety: "never test or experiment directly in a live Production environment".

---

## Takeaways and Practical Application

### Key Learnings
*   **Tech & Security Insights:** Gained easy value on Containerization with Docker, real-time bi-directional WebSockets communication in gaming, ML applications in intrusion detection, and GraphRAG's entity-linking capabilities.
*   **Collaboration & Growth:** Mastered the 4 golden rules of teamwork to apply in collaborative projects, and shaped a self-study mindset to build a robust career path.

### Work Integration
*   **Container Packaging:** Apply Docker to current academic projects to unify development environments and deliver applications quickly.
*   **Real-time & AI Experiments:** Research integrating API Gateway's WebSocket APIs for applications requiring continuous state updates, and explore GraphRAG with Amazon Bedrock.
*   **Management & Operations:** Utilize teamwork principles and digital tools like Slack/Trello to manage project timelines during the bootcamp, maintaining system operation discipline.

---

## Personal Experience & Impressions

The meetup provided an extremely dynamic and valuable space for networking and knowledge exchange:

*   **Diverse Range of Topics:** Presentations covered everything from infrastructure, game development, and cybersecurity, to soft skills and career growth stories.
*   **High Practicality:** Real-world experiences from Vinh Trần and practical solutions from other speakers broadened my perspective and gave me immense motivation to self-study.

### Event Photos

![Check-in at the event](/images/4-Eventparticipated/event2.jpg)

> Overall, the event brought me modern technical knowledge and highly valuable career lessons to confidently move forward on the DevOps/Sysadmin path.
