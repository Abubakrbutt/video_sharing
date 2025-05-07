# Video Transcript for InstaShare Demo

## [0:00 - 0:20] Introduction
Hello everyone. My name is Abu bakar and today I will show you PhotoShare, a scalable photo sharing platform I built using cloud technologies. This platform is similar to Instagram, allowing creators to upload photos while consumers can view, like, and comment on them.

## [0:20 - 0:49] Technology Stack and Problem Statement
For this application, I've used Django for the backend with Python 3.12, MySQL for the database, and Bootstrap with custom CSS for the frontend. Photo sharing platforms like Instagram face significant scalability challenges - they need to handle millions of users, store large amounts of media efficiently, and deliver content quickly across the globe. Traditional approaches often fail when user numbers surge or storage requirements explode.

## [0:50 - 1:15] Scalability Issues
The main scalability issues with photo sharing applications include rapidly growing storage needs as users upload content, database performance degradation with increased user interactions, authentication bottlenecks during peak usage times, and the need for global content delivery. My solution addresses these using cloud-native components in Azure that can scale independently as needed.

## [1:16 - 1:47] Azure MySQL Configuration
Let's look at our Azure deployment. First, here's the Azure MySQL database service I've configured for our application. I've chosen a flexible server option which allows scaling compute and storage resources independently. You can see the database that i have created for our application. Using Azure's managed MySQL service provides benefits like automatic backups, high availability, and the ability to scale without application downtime.

## [1:48 - 2:18] Azure App Service Configuration
Now let's examine the App Service where our application is deployed. Here you can see I've configured the runtime stack as Python 3.12. App Service provides several scalability benefits including automatic scaling based on demand, load balancing, and global distribution capabilities. These features ensure our application remains responsive even during traffic spikes without requiring manual intervention.

## [2:19 - 2:57] Deployment Strategy
In the deployment center, you can see I've configured external Git as our deployment strategy. Unlike CICD pipelines that automatically deploy code whenever changes are pushed, I've chosen manual sync for greater control. This allows me to verify changes before deploying to production. Unlike FTP where you must track and upload changed files individually, Git tracks all changes automatically, making deployment much simpler and less error-prone. Let me show how I can deploy changes with a single sync action.

## [2:58 - 3:26] Application Registration and Login
Now let's look at the application interface. Here's the registration page where users can create accounts by providing a username, email, password, and by default user is created as consumer only admin can change a consumer role to creator from the Django Admin panel. 

## [3:27 - 3:53] Creator Interface
Here's the creator interface where creators can see their uploaded content. Creators have exclusive access to the upload functionality via this button in the navigation bar. Let me show you the upload form where creators can add a photo, title, caption, location information, and people present in the photo. This metadata enhances searchability and user engagement.

## [3:54 - 4:22] Consumer Interface
Switching to the consumer interface, users see a feed of photos they can browse through. Consumers can interact with content by rating photos and using the comment section. Notice how quickly the images load due to our efficient storage. Consumers can also view detailed information about each photo including location and people present, and see all associated comments.


## [4:22 - 4:36] Scalability Benefits
Let me highlight how our architecture addresses scalability. The Azure App Service automatically scales instances based on traffic. Our database can grow as needed without application changes. 

## [4:37 - 5:00] Conclusion
In conclusion, I've successfully built a scalable, cloud-native photo sharing platform that addresses the key challenges of media distribution applications. By leveraging Azure's managed services and implementing proper role-based access control, the solution demonstrates both technical excellence and practical application of scalable design principles.