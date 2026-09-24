# Mission Reflection

Object storage is better suited for storing millions of photos because photos are unstructured data. Unlike block storage, object storage is designed to handle many files while keeping each file with its data and metadata. It can also scale as more photos are added, so the system does not depend on one hard drive. For a photo-sharing application, this makes storage easier to manage as the number of users and images grows.

Using Docker made deploying MinIO much easier because I did not have to manually install and configure every part of the storage server. I only needed to run the Docker command with the ports, username, password, and MinIO image. Docker handled the container setup for me, which made the process faster and easier to manage. It was easier to restart or manage the server.

A bucket in cloud storage is like a main container where objects are stored. In this activity, I created a bucket named client-photos and uploaded our sample file inside it. The bucket helps organize the stored objects and gives the application a specific place for saving and accessing files. It also makes data easier to manage.

Large enterprise companies can protect object storage data from being lost by keeping multiple copies of the data in different servers and locations. They can also use replication, backups, and systems that automatically move or recover data when a server fails. This means that even if one server crashes, another copy of the data can still be available. These methods help reduce the risk of data loss.

My confidence in using the Linux command line is growing because I was able to follow the commands and understand them. At first, Docker commands were confusing, especially when an error appeared. After fixing the command and successfully running MinIO, I became more comfortable using the terminal. This activity helped me realize that I can learn command-line tasks through practice and by understanding each command instead of simply copying everything alone.
