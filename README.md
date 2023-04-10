# 🖥️  On-Premise 3-tier Architecture Project

PROmet On-Premise Infrastructure 구축 프로젝트는 이직 platform인 PROmet 웹사이트를 구축하는 것이 목표입니다. 이직 정보나 구인 정보를 검색하는 과정에서 겪는 어려움을 극복하고자, 이직 platform을 제공합니다. 근로자의 경력과 전문성에 맞게 게시글과 이력서, 포트폴리오, 자기소개서 등을 등록하면, 파트너 기업에서 고용주들이 스카우트 제안을 보낼 수 있도록 연결합니다. 이를 통해 근로자들은 더 나은 기회를 찾을 수 있고, 기업은 핵심 업무에 맞게 적합한 인재를 쉽게 구할 수 있습니다.

![image](https://user-images.githubusercontent.com/76054852/230912393-54f73945-a501-4db3-8281-8e6c88b4eb47.png)


## Objective

The objective of this On-Premise 3-tier Infrastructure was to build the PROmet job search website, which connects job seekers with potential employers. PROmet provides a platform for job seekers to register their resumes, portfolios, and self-introductions. Partner companies can then scout potential candidates who fit their needs, providing both job seekers and employers with better opportunities.


## Goals and Design
The project was divided into several parts. First, we implemented a Django-based system to allow job seekers to register their resumes, portfolios, and self-introductions. We used several technologies, including Apache, HAProxy, GlusterFS, MariaDB, and OpenSSL, to accomplish this. We then deployed WEB/WAS servers, created and connected GlusterFS servers, and connected Proxy, DNS, and DB servers to build an on-premise infrastructure, as shown in the picture. My role in the project included proposal and planning, Django app creation, WAS server deployment, GlusterFS server creation and connection, and Proxy, DNS, and DB server integration. I designed each server and solution, then connected them to build a stable infrastructure. Finally, I wrote a shell script to monitor and manage each server.

## Conclusion

This project taught me how to use various technologies and solutions to build an on-premise 3-Tier infrastructure. I also learned how to solve problems that arise when connecting each server. Although there were many challenges during the project, one significant issue was configuring the Slave DB server to replicate as a read-only replica. We solved this problem by adding a Python file to the Django project to route read-only traffic to the Slave DB and other operations to the Master DB. This significantly reduced the load on the Master DB and distributed the load of read operations to the Replication Slave DB. Through this technical problem-solving process, I acquired new skills and solutions, enabling me to develop better capabilities.
