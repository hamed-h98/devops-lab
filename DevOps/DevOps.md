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




























