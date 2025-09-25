# Introduction-to-Jenkins
Here’s a **brief introduction to Jenkins**:

---

**Jenkins** is an **open-source automation server** widely used for **Continuous Integration (CI) and Continuous Delivery (CD)**. It helps developers and DevOps engineers automate the process of building, testing, and deploying applications. Instead of manually running scripts every time code changes, Jenkins automatically pulls updates from version control systems like Git, builds the application, runs tests, and then deploys it to servers or containers.

Key advantages of Jenkins include:

* **Automation** → Reduces manual work in build, test, and deployment.
* **Plugins** → Supports hundreds of integrations (Docker, Kubernetes, AWS, GitHub, etc.).
* **Scalability** → Can run jobs on multiple nodes for distributed builds.
* **Flexibility** → Works with many programming languages and environments.

In simple terms: Jenkins acts as the **central hub** for automating the software delivery pipeline, ensuring faster releases, fewer errors, and more reliable deployments.

---
Lets install Jenkins and set the server to handle automations. 
1. Spin up a jenkins server and update with recent dependencies and packages. Verify that Jenkins is active with 'sudo systemctl status jenkins'

   <img width="954" height="381" alt="image" src="https://github.com/user-attachments/assets/127868ea-83cc-413f-86e7-0cb14d28d476" />
   <img width="799" height="280" alt="image" src="https://github.com/user-attachments/assets/8732c768-1400-4661-aee5-b690c5a0f68a" />
   <img width="964" height="503" alt="image" src="https://github.com/user-attachments/assets/b0671f9e-435a-4609-844e-6a64cda0ee47" />
   <img width="962" height="484" alt="image" src="https://github.com/user-attachments/assets/e2e8ba54-c531-49f0-8209-67a79607795b" />
   <img width="953" height="500" alt="image" src="https://github.com/user-attachments/assets/41e4d4d6-3745-4917-973e-f18ce1b8fa28" />


2. On the Jenkins instance EC2, open port 8080 and connect to it using the public IP address.
   <img width="959" height="401" alt="image" src="https://github.com/user-attachments/assets/1cd26b01-e94f-4c78-a5d2-78a4ae157e45" />
   <img width="931" height="380" alt="image" src="https://github.com/user-attachments/assets/900ef268-d1e0-4986-8d73-04891aa0465c" />
   <img width="946" height="391" alt="image" src="https://github.com/user-attachments/assets/8d81618c-fe92-4d4d-850f-baffc356a5ad" />
   <img width="956" height="484" alt="image" src="https://github.com/user-attachments/assets/a653a405-c21d-442e-8781-0f38886d6afb" />

3. Retrieve the password using cat command and login to jenkins.Install suggested plugins.
   <img width="962" height="322" alt="image" src="https://github.com/user-attachments/assets/d3f26e42-621d-4557-b449-4e6ef4a1b4a6" />
   <img width="792" height="419" alt="image" src="https://github.com/user-attachments/assets/cdcfddd8-bb9c-42b1-ad7d-9e4f36da99c2" />
   <img width="769" height="430" alt="image" src="https://github.com/user-attachments/assets/4b423eed-9b3d-46db-9632-a0d4572d0232" />
   <img width="954" height="451" alt="image" src="https://github.com/user-attachments/assets/f6e3a135-1f60-4de8-a93f-ee1af05e7db1" />











