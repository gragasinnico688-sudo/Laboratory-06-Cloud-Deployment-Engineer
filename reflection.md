# Mission 5 Reflection

This laboratory activity helped me understand why object storage is useful for applications that need to store a large number of files. Object storage is better suited for millions of photos because it is designed for unstructured data such as images, videos, and backups. Instead of treating every file like a traditional hard drive, object storage keeps files as objects inside buckets and can scale as the amount of data increases. This makes it a practical choice for a photo-sharing application.

Docker made deploying MinIO easier because I did not need to manually install and configure all of the required software. I was able to use one Docker command to download the MinIO image, create the container, configure the login credentials, and expose the required ports. This was faster and more convenient compared to setting up a complete server manually.

A bucket is a logical storage container used to organize objects in object storage. In this activity, the bucket was named `client-photos`, and I uploaded a sample file to it. The bucket gives the application a specific place where uploaded photos can be stored and managed.

Large enterprise companies use different methods to protect object storage data from being lost when physical hardware fails. They can keep multiple copies of data, replicate information across different servers or locations, and use backups and redundancy. Cloud providers also use durable storage systems so that hardware failure does not automatically mean that the stored data is lost.

My confidence with the Linux command line is also improving. In the previous laboratory, I worked with Docker commands to run an Nginx container. In this activity, I used Docker again to deploy MinIO and check its status. I am becoming more comfortable entering commands, reading terminal output, and troubleshooting when something does not work immediately. My GitHub portfolio is also growing because each laboratory adds another practical cloud computing skill and documented project.
