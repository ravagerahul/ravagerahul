<img src="https://capsule-render.vercel.app/api?type=venom&color=0:00f5a0,50:00b8d9,100:7928ca&height=230&section=header&text=Rahul%20Walia&fontSize=62&fontColor=ffffff&animation=twinkling&fontAlignY=40&desc=Backend%20Engineer%20%E2%80%A2%20Event-Driven%20Systems%20%E2%80%A2%20Cloud&descAlignY=62&descSize=18" width="100%" alt="header"/>

<div align="center">

[![Typing SVG](https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=21&pause=900&color=00F5A0&center=true&vCenter=true&width=700&height=40&lines=%24+whoami+%E2%86%92+Rahul+Walia;%24+stack+%E2%86%92+Java+%C2%B7+Spring+Boot+%C2%B7+Kafka+%C2%B7+AWS;%24+building+%E2%86%92+event-driven+systems+with+LLMs;%24+learning+%E2%86%92+Golang;%24+status+%E2%86%92+open+to+opportunities)](https://github.com/ravagerahul)

<a href="https://www.linkedin.com/in/rahulwalia2/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white"/></a>
<a href="mailto:riitwalia38@gmail.com"><img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white"/></a>
<img src="https://komarev.com/ghpvc/?username=ravagerahul&label=VIEWS&color=00b8d9&style=for-the-badge"/>

</div>

---

## `~/about.sh`

```java
public class Rahul extends FullStackDeveloper implements BackendEngineer {

    String   location   = "India";
    String[] coreStack  = { "Java 17", "Spring Boot 3", "Kafka", "PostgreSQL", "AWS" };
    String[] frontend   = { "React", "TypeScript", "JavaScript" };
    String[] devops     = { "Docker", "Kubernetes", "Jenkins", "Caddy" };

    String currentlyBuilding = "SpendSense AI - SMS -> Kafka -> LLM -> Postgres pipeline";
    String currentlyLearning = "Golang, distributed systems, RAG";
    String funFact           = "I solve DSA problems daily in C++";

    public boolean openToWork() { return true; }
}
```

## ⚡ Flagship Project: SpendSense AI

> Turns the bank SMS that already lands on your phone into a **categorized, queryable spending history**. UPI apps expose no API, so the SMS is the one reliable channel.

```mermaid
flowchart LR
    A[iOS Shortcut] -->|POST SMS| B[ingestion-service]
    B -->|raw-sms-received| K1{{Kafka}}
    K1 --> C[extraction-service<br/>LLM parsing]
    C -->|transaction-extracted| K2{{Kafka}}
    K2 --> D[storage-service<br/>Postgres + pgvector]
    D -->|transaction-stored| K3{{Kafka}}
    K3 --> E[categorization-service]
    K3 --> F[anomaly-service]
    D --> G[dashboard-service BFF]
    G --> H[React dashboard]
    G --> I[query-service<br/>NL chat + vector search]
```

| | |
|---|---|
| 🏗️ **Architecture** | 8 Spring Boot microservices in a Gradle multi-module build, communicating over Kafka |
| 🧠 **AI** | LLM extracts amount, merchant, direction and date from raw SMS; embeddings in **pgvector** power natural-language chat |
| 🔒 **Privacy** | Account balances are masked before text ever reaches the model |
| 🛡️ **Reliability** | Correlation IDs trace each message end to end; 3 failed attempts route to a dead-letter topic instead of losing data |
| 🚢 **Deploy** | Docker Compose with Caddy as the single entry point |
| 📦 **Codebase** | ~150k lines of Java, ~65k of TypeScript |

[![Repo](https://img.shields.io/badge/View%20Repo-SpendSense%20AI-00f5a0?style=for-the-badge&logo=github&logoColor=black)](https://github.com/ravagerahul/SpendSense-AI-Event-Driven-Personal-Finance-Intelligence-Platform)

## 🛠️ Tech Arsenal

<div align="center">

![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white)
![Kafka](https://img.shields.io/badge/Kafka-231F20?style=flat-square&logo=apachekafka&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)
![DynamoDB](https://img.shields.io/badge/DynamoDB-4053D6?style=flat-square&logo=amazondynamodb&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonwebservices&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white)
![Jenkins](https://img.shields.io/badge/Jenkins-D24939?style=flat-square&logo=jenkins&logoColor=white)
![Gradle](https://img.shields.io/badge/Gradle-02303A?style=flat-square&logo=gradle&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white)
![C++](https://img.shields.io/badge/C++-00599C?style=flat-square&logo=cplusplus&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Go](https://img.shields.io/badge/Go-00ADD8?style=flat-square&logo=go&logoColor=white)

</div>

## 📂 More Projects

| Project | Description | Stack |
|---|---|---|
| [🧬 **GPS Dementia Patient Monitoring**](https://github.com/ravagerahul/GPS-based-Alzheimer-dementia-patientmonitoring-system) | Real-time GPS tracking system to monitor Alzheimer's and dementia patients | `Java` |
| [🧮 **DSA**](https://github.com/ravagerahul/DSA) | Daily data structures and algorithms practice | `C++` |
| [📚 **Library Management System**](https://github.com/ravagerahul/library-management-system) | Web app to manage books and members | `HTML` |
| [✅ **Todo App**](https://github.com/ravagerahul/todo-app) | Task manager with a clean UI | `JavaScript` |

## 📊 GitHub Analytics

<div align="center">

<img height="165" src="https://github-readme-stats.vercel.app/api?username=ravagerahul&show_icons=true&theme=radical&hide_border=true&count_private=true" alt="stats"/>
<img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=ravagerahul&layout=compact&theme=radical&hide_border=true" alt="top languages"/>

<img src="https://streak-stats.demolab.com?user=ravagerahul&theme=radical&hide_border=true" alt="streak"/>

</div>

## 🤝 Let's Build Something

I'm looking for backend and full stack roles where I can work on distributed, event-driven systems. If you're hiring or want to collaborate, reach out on [LinkedIn](https://www.linkedin.com/in/rahulwalia2/) or [email me](mailto:riitwalia38@gmail.com).

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:7928ca,50:00b8d9,100:00f5a0&height=110&section=footer" width="100%" alt="footer"/>
