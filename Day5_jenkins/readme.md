### Question/Answer

### Ques.What are webhooks and GitHub webhooks
Ans. A webhook (also called a web callback or HTTP push API) is a way for an app to provide other applications with real-time information. A webhook delivers data to other applications as it happens, meaning you get data immediately. Webhooks allow you to build or set up integrations, such as GitHub Apps or OAuth Apps, which subscribe to certain events on GitHub.com. When one of those events is triggered, we'll send a HTTP POST payload to the webhook's configured URL. Webhooks can be used to update an external issue tracker, trigger CI builds, update a backup mirror, or even deploy to your production server.

### Ques.How to give git credentials in Jenkins
Ans. Select “Git” for Source Code ManagementClick on “Git” to select it. This will expand the section, and show all git related By default, this will be “None”. There will be an “Add” button next to it. From here, you can specify the credentials that are required for the Git URL specified above.

### Ques.How to use private git repositories in jenkins freestyle project
Ans.Go to Jenkins dashboard -> Credentials -> System -> Global credentials -> Add credentials. Give the username as Jenkins or whatever you can remember. Add the Private key -> Enter directly and copy paste the same ssh keys here, click on okay.

### Ques.ls continuous delivery and Continuous Deployment alternate process?
Ans.Continuous Delivery is the frequent shipping of code to a given environment (such as test or production) via manual release. Continuous Deployment is the automated release of code to a production environment.

### Ques.What is monitoring
Ans.Continuous Monitoring is an automated process that leverages specialized software tools to empower DevOps teams with enhanced visibility of application performance, security threats, and compliance concerns across the entire DevOps pipeline.

### Ques.What is credential in Jenkins
Ans.To maximize security, credentials configured in Jenkins are stored in an encrypted form on the controller Jenkins instance (encrypted by the Jenkins instance ID) and are only handled in Pipeline projects via their credential IDs.

