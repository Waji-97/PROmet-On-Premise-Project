# 🖥️  On-Premise 3-tier Architecture Project

The objective of this On-Premise 3-tier Infrastructure was to deploy the PROmet job search website to the on-premise infrastructure. PROmet provides a platform for job seekers to register their resumes, portfolios, and self-introductions. Partner companies can then scout potential candidates who fit their needs, providing both job seekers and employers with better opportunities.

![image](https://user-images.githubusercontent.com/76054852/230912393-54f73945-a501-4db3-8281-8e6c88b4eb47.png)

> Technical Documentation and a Presentation pdf files are included

---

## ⛏️ Goals and Design
The project was divided into several parts. First, we implemented a Django-based system to allow job seekers to register their resumes, portfolios, and self-introductions. We used several technologies, including Apache, HAProxy, GlusterFS, MariaDB, and OpenSSL, to accomplish this. We then deployed WEB/WAS servers, created and connected GlusterFS servers, and connected Proxy, DNS, and DB servers to build an on-premise infrastructure, as shown in the picture. My role in the project included proposal and planning, Django app creation, WAS server deployment, GlusterFS server creation and connection, and Proxy, DNS, and DB server integration. I designed each server and solution, then connected them to build a stable infrastructure. Finally, I wrote a shell script to monitor and manage each server.

## 📝 Conclusion

This project taught me how to use various technologies and solutions to build an on-premise 3-Tier infrastructure. I also learned how to solve problems that arise when connecting each server. Although there were many challenges during the project, one significant issue was configuring the Slave DB server to replicate as a read-only replica. We solved this problem by adding a Python file to the Django project to route read-only traffic to the Slave DB and other operations to the Master DB. This significantly reduced the load on the Master DB and distributed the load of read operations to the Replication Slave DB. Through this technical problem-solving process, I acquired new skills and solutions, enabling me to develop better capabilities.
