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


   Before proceeding to use jenkins, you would have to intergrate a desired SCM with Jenkins. in this case, we choose github.
   <img width="952" height="318" alt="image" src="https://github.com/user-attachments/assets/f41d628b-e5ef-42cf-a105-fe12d375c006" />
   <img width="940" height="430" alt="image" src="https://github.com/user-attachments/assets/600b7e08-ed8c-4bb9-ae01-092468d99c0a" />
   <img width="714" height="346" alt="image" src="https://github.com/user-attachments/assets/5363c1fb-8e4d-4ce5-802b-00c3bbfae219" />
   <img width="935" height="431" alt="image" src="https://github.com/user-attachments/assets/8640397d-501d-452e-9dc2-20a67c522eb5" />
   <img width="959" height="445" alt="image" src="https://github.com/user-attachments/assets/cec2a092-e40f-4ddc-a72a-7f9d3f81b935" />
   <img width="944" height="440" alt="image" src="https://github.com/user-attachments/assets/d118190d-e6c5-4813-ae2b-17c094d19221" />
   <img width="655" height="323" alt="image" src="https://github.com/user-attachments/assets/131adbf6-3402-490b-a70b-83052b2a4d03" />
   <img width="696" height="349" alt="image" src="https://github.com/user-attachments/assets/17efff96-0f6f-47a8-abce-f29c89f8ccd9" />
   <img width="951" height="379" alt="image" src="https://github.com/user-attachments/assets/9c633ab4-a900-47a2-a4e3-f98556129663" />
   <img width="959" height="433" alt="image" src="https://github.com/user-attachments/assets/247bf97c-b638-4ecf-b94d-c9f4a5a72834" />
   <img width="959" height="428" alt="image" src="https://github.com/user-attachments/assets/cd3b3a0f-b58a-4ec1-afb0-0f1f97dbcd80" />
   <img width="958" height="430" alt="image" src="https://github.com/user-attachments/assets/e6b11ef3-2cd5-48e4-8ff1-112dc04d6c86" />
   <img width="956" height="442" alt="image" src="https://github.com/user-attachments/assets/396ad65c-db26-48fe-9566-4fde7191dab3" />
   <img width="955" height="431" alt="image" src="https://github.com/user-attachments/assets/819aadf2-1283-4309-aef6-5165e370c697" />














5. Create and Run a Freestyle Job.
   i. Log into Jenkins → Dashboard → New Item. Choose Freestyle Project, give it a name (my-first-job).

  ii. In the configuration:
      Add a description.
      Under Source Code Management (SCM) → select Git.
      Enter your repo URL (e.g., GitHub HTTPS/SSH).
      Provide credentials if private.
      Under Build Triggers → choose “Build periodically” or “Poll SCM” if you want automation.
     Under Build → add a simple command (like echo "Hello Jenkins").
  iii. Save and Build Now.
   Check the console output to verify success.
   
Below are the images with the demo
<img width="944" height="470" alt="image" src="https://github.com/user-attachments/assets/f783f54a-8cb1-424c-ac7c-4b92b70e0b2d" />
<img width="945" height="436" alt="image" src="https://github.com/user-attachments/assets/2c638064-4627-4575-96f5-f2ba3f53c7db" />
<img width="956" height="439" alt="image" src="https://github.com/user-attachments/assets/bddf89d1-1a25-416b-95f0-a950ec1d6554" />
<img width="949" height="440" alt="image" src="https://github.com/user-attachments/assets/70fd78ec-8445-40e0-9f88-9dc8c504cf91" />









