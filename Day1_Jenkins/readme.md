CI/CD - Question/Answer


### Q-1 What are webhooks and GitHub webhooks?

A-1 A webhook (also called a web callback or HTTP push API) is a way for an app to provide other applications with real-time information. A webhook delivers data to other applications as it happens,
 meaning you get data immediately.

Webhooks allow you to build or set up integrations, such as GitHub Apps or OAuth Apps, which subscribe to certain events on GitHub.com. When one of those events is triggered, we'll send a 
HTTP POST payload to the webhook's configured URL. Webhooks can be used to update an external issue tracker, trigger CI builds, update a backup mirror, or even deploy to your production server.


### Q-2  How to give git credentials in Jenkins?

A-2 Select “Git” for Source Code Management
Click on “Git” to select it. 
This will expand the section, and show all git related
By default, this will be “None”. There will be an “Add” button next to it. From here, you can specify the credentials that are required for the Git URL specified above.


### Q-3 How to use private git repositories in the Jenkins freestyle project ?

A-3 Go to Jenkins dashboard -> Credentials -> System -> Global credentials -> Add credentials. Give the username as Jenkins or whatever you can remember. Add the Private key -> Enter directly and
 copy paste the same ssh keys here, click on okay.


### Q-4 Is Continuous delivery and Continuous Deployment alternate process ?

A-4 Continuous Delivery is the frequent shipping of code to a given environment (such as test or production) via manual release.
 Continuous Deployment is the automated release of code to a production environment.


### Q-5 Packaging is a part of CI or CD ?

A-5


### Q-6 What is Monitoring ?

A-6 Continuous Monitoring is an automated process that leverages specialized software tools to empower DevOps teams with enhanced visibility of application performance, security threats, 
and compliance concerns across the entire DevOps pipeline.


### Q-7 What is credential in Jenkins ?

A-7 To maximize security, credentials configured in Jenkins are stored in an encrypted form on the controller Jenkins instance (encrypted by the Jenkins instance ID) and are only handled in 
Pipeline projects via their credential IDs.
