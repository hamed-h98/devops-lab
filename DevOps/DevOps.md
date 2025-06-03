# DevOps

#### Source: https://www.youtube.com/watch?v=0yWAtQ6wYNM

<img src="images/image1.png" alt="Alt text" width="300">

DevOps is something between development and operations 

<img src="images/image2.png" alt="Alt text" width="400">

The main goal: 
- APP ---> deliver application to end usr 

<img src="images/image3.png" alt="Alt text" width="500">


Configure the server:
- Installing tools
- Deploy application
- Configure Firewall 


<img src="images/image4.png" alt="Alt text" width="500">


<img src="images/image5.png" alt="Alt text" width="500">


#### To keep track of updates (changes), we version those changes. 

<img src="images/image8.png" alt="Alt text" width="600">


For versioning, we have a template and rule: 

e.g., `1.4.2`

`1` is for major changes 
`4` minor changes (editing one small feature)
`2` one for quick small changes (bugfix) 


<img src="images/image9.png" alt="Alt text" width="700">


#### DevOps is for making this continuous devilery fast with minimal bugs. 


<img src="images/image10.png" alt="Alt text" width="700">


Quickly delivering high quality code is a big challenge. 

Challenges in the release process: 

- Misscommunication and lack of collaboration between developers and operations 

    * code the application (Developers)
    * Deploy and operate the application (operations for running the application) 

<img src="images/image11.png" alt="Alt text" width="600">

Deployment guide not well documented. so the release takes longer. Or developers finish coding but the feature cannot be deployed because it has lot of issues and the operations throws it back with improvement suggestions. 

This kind of misscommunication could cause streching the release periods for days, weeks or months. 

So between developer is done with the feature and operation starts deploying it, there is no clearly defined automated process of handover. It's based on a complex bureaucratic process of what checklists need to be completed and what needs to be documented and who needs to manually approve what for the release and so on. 

So steamlines and automated process is here. 

#### 2- Conflict of Interest 

<img src="images/image12.png" alt="Alt text" width="600">

Operations want to make sure changes won't break anything. Operations want to maintain stability in production and their focus is to make sure application is available and does not crash. So operations need to resist the speed of release and check all aspects of new release to make sure it's 100% safe which this slows down the process. Especially that the operations don't really understand the code or the applications, so there is more effort for them to evaluate this new release. 


For example let's say developers developed a new feature which was released, but this feature consumes so much resources in the production environment that the servers got overloaded and the application crashed. Now operations team needs to fix that. So the developers may not be careful as the operations about the changes they releasse. 

<img src="images/image13.png" alt="Alt text" width="600">


Also security team will evaluate any changes to make sure they don't effect system's security. 

<img src="images/image14.png" alt="Alt text" width="600">

So these procedures slows down the process. So the DevOps is about to remove any roadblocks that slow down the process. so the security is also part of the DevOps. But there is a separate term of security is defined for DevOps and it's called DevSecOps 

<img src="images/image15.png" alt="Alt text" width="600">


<img src="images/image16.png" alt="Alt text" width="500">

This testing may not be done by the Development or Operations rule but with a separate Testing rule. 

<img src="images/image17.png" alt="Alt text" width="400">

<img src="images/image18.png" alt="Alt text" width="500">

This testing is also slowing down the process since these tests are done manually. 

<img src="images/image19.png" alt="Alt text" width="500">

This manual work is slow and more error-prone. 

Plus with the manual work, knowledge sharing is difficult. Because people have to document it and others have to read it. 

It's also very intransparent cause it's hard to trace, who execute what when. 

Also if something happens to the infrastructure, it maybe really hard to recover and replicate the exact state fast. 

<img src="images/image20.png" alt="Alt text" width="500">


<img src="images/image21.png" alt="Alt text" width="200">


DevOps tries to remove these roadblocks and things that slow down the release process. 


<img src="images/image22.png" alt="Alt text" width="500">


Many companies, implemented DevOps in different ways. But some patterns are common. 


<img src="images/image23.png" alt="Alt text" width="500">


One of these patterns was that devops evolved into an actual role called DevOps engineer. 

And the technologies used to implement the DevOps principles are called devops techonologies. 

In the center of DevOps, we have CI/CD. 


<img src="images/image24.png" alt="Alt text" width="500">

---

### Concepts of Software Development 


<img src="images/image25.png" alt="Alt text" width="300">


A DevOps engineer does not program the application, but he/she must understand how the developers work, which Git workflow they are using. Also how the application configured to talk to other services or data bases and also the concepts of automated testing. 

---

#### Operating systems and linux Basics 

After the development (coding and Git), the application needs to be deployed on a server so users can access it. So we need some kind of infrastructure on-premis servers or cloud servers. These servers needs to be created abd configured to run our application. 

A DevOps engineer maybe responsible to prepare the infrastructure to run the application. 

Most of the servers are applications that are running on Linux servers, then a DevOps engineer must know Linux. Also he/she needs to be comfortable using command line interface (CLI) (terminal). 


<img src="images/image26.png" alt="Alt text" width="500">

Installing tools and software on servers, Linux file system, server management, SSH key management are essential. 

Also DevOps engineer must know basics of Networking and Security. 

To configure firewalls to secure the application, open some ports to make application accessible from outside. 

<img src="images/image27.png" alt="Alt text" width="200">

The advanced operating system, or networking and security is not needed for DevOps engineer. 

For System Administrator, Network and Security, there are special engineers for each of these fields. 

---

### Containers


<img src="images/image28.png" alt="Alt text" width="400">

We are going to run the application as containers on a server. So we need to understand Virtualization and Containers and managing containerized applications on a server. 

Docker is a container technology that we need to learn. 

#### How to release application? 

How to make the application accessible to users from development and repository, to servers and having multiple versions of the application. 

In DevOps way, this must be done continuously (CI/CD) in an efficient and fast (Automated) way. 

---

### Build Automatio & CI/CD

When the tests are done, we need to package the application as an artifact like JAR file for Zip so that we can deploy it. 

For example for package management, we have Maven or Gradle in Java, npm for javascript 

Then we need to make a Docker image for the application and this image must be saved in an imagerepository. So Docker artifact repository on Nexus or dockerhub will be used here. 

We want one pipeline that does all of this in sequential step (automated). So we need to build automation using GitLab, Jenkins, Github Actions, TeamCity 


<img src="images/image29.png" alt="Alt text" width="500">


There maybe some additional steps in the above pipline like sending notifications to the team about the pipline state or handling fail deployment. But this is the core CI/CD pipline. 

CI/CD pipline is the heart of the devops tasks and responsibility. 

<img src="images/image30.png" alt="Alt text" width="500">

---

### Cloud Providers 










