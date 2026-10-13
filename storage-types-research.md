# Storage Types Research

## Block, File, and Object Storage

| Storage Type | Description | Primary Use Case | Cloud Provider Example |
|---|---|---|---|
| Block Storage | Stores data in fixed-size blocks that can be attached to a server like a virtual hard drive. | Operating systems, databases, and applications that need fast disk access. | AWS EBS |
| File Storage | Stores data as files organized into folders and directories that can be shared over a network. | Shared files, documents, and applications that need a common file system. | AWS EFS |
| Object Storage | Stores data as objects together with metadata and a unique identifier inside a storage bucket. | Images, videos, backups, documents, and other large amounts of unstructured data. | Amazon S3 |

## Why Object Storage for User Photos?

Object Storage is a good choice for the client's photo-sharing application because it is designed to store large amounts of unstructured data such as images and videos. It can also scale as the number of uploaded photos increases without requiring the application server to store all of the files locally. This makes Object Storage more suitable for a photo-sharing service with potentially millions of user-uploaded images.
