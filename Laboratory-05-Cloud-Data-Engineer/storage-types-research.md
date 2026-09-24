# Storage Types Research

| Storage Type       | Description                                                                         | Primary Use Case                                                                       | Cloud Provider Example |
| ------------------ | ----------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- | ---------------------- |
| **Block Storage**  | Stores data in fixed-size blocks that can be accessed individually.                 | Best for virtual machines, databases, and applications that need fast data access.     | AWS EBS                |
| **File Storage**   | Stores data as files in folders and directories that can be shared over a network.  | Best for shared files, documents, and applications that need access to the same files. | AWS EFS                |
| **Object Storage** | Stores data as objects together with their data, metadata, and a unique identifier. | Best for images, videos, backups, and other large unstructured data.                   | AWS S3                 |

### Why Object Storage?

Object Storage is the best choice for the client's photo-sharing application because it is designed to store large amounts of unstructured data such as user-uploaded images. It can also scale easily as the number of photos increases, making it suitable for storing millions of images.

