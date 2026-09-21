# Mission Reflection

In this laboratory activity, I learned why object storage is more suitable for storing millions of photos compared to traditional block storage. Object storage is designed to handle large amounts of unstructured data such as images, videos, backups, and documents. Each object can also have metadata, making the data easier to organize and manage. For a photo-sharing application that may contain millions of user uploads, object storage provides a more scalable solution.

Using Docker also made deploying the MinIO storage server easier. Instead of manually installing and configuring MinIO and its dependencies, I was able to start the server using a Docker command. The command allowed me to configure the ports, administrator credentials, and storage location. I also learned how to verify that the container was running using the `docker ps` command.

A bucket in cloud object storage is a container used to organize and store objects. In this activity, I created the `client-photos` bucket and uploaded a sample image through the MinIO Web Console. This helped me understand how cloud applications can organize uploaded files separately from the application server itself.

Large enterprise companies can protect object storage data by keeping multiple copies of data across different storage systems, servers, or locations. Replication, backups, redundancy, and disaster recovery strategies can help ensure that data remains available even if a physical server or storage device fails.

My confidence in using the Linux command line is also improving. I am becoming more comfortable navigating directories, checking files, running Docker commands, viewing logs, and using Git commands to save my work. I still need practice with some commands, but completing these activities step by step has helped me better understand how Linux is used in cloud computing.
