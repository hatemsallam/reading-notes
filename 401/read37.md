# S3

* Amazon Simple Storage Service (Amazon S3) is storage for the Internet. It is designed to make web-scale computing easier.

* Amazon S3 has a simple web services interface that you can use to store and retrieve any amount of data, at any time, from anywhere on the web.
* It gives any developer access to the same highly scalable, reliable, fast, and inexpensive data storage infrastructure that Amazon uses to run its own global network of web sites.

## Advantages of using Amazon S3

* Creating buckets
* Storing data
* Downloading data
* Permissions
* Standard interfaces

## Amazon S3 concepts

* A bucket is a container for objects stored in Amazon S3.
* Every object is contained in a bucket.
* Buckets serve several purposes:
  * They organize the Amazon S3 namespace at the highest level.
  * They identify the account responsible for storage and data transfer charges.
  * They play a role in access control.
  * They serve as the unit of aggregation for usage reporting.

* Objects are the fundamental entities stored in Amazon S3
* Objects consist of object data and metadata.
* The data portion is opaque to Amazon S3.
* The metadata is a set of name-value pairs that describe the object.
* A key is the unique identifier for an object within a bucket.
* Every object in a bucket has exactly one key.
* The combination of a bucket, key, and version ID uniquely identify each object.

## Amazon S3 data consistency model

* Amazon S3 provides strong read-after-write consistency for PUTs and DELETEs of objects in your Amazon S3 bucket in all AWS Regions.
* Bucket configurations have an eventual consistency model. Specifically:
  * If you delete a bucket and immediately list all buckets, the deleted bucket might still appear in the list.
  * If you enable versioning on a bucket for the first time, it might take a short amount of time for the change to be fully propagated.

  ## Amazon S3 features

  * Storage classes : Amazon S3 offers a range of storage classes designed for different use cases.
  * Bucket policies : provide centralized access control to buckets and objects based on a variety of conditions, including Amazon S3 operations, requesters, resources, and aspects of the request (for example, IP address). 
  * AWS Identity and Access Management :You can use it to manage access to your Amazon S3 resources.
  * Access control lists: You can control access to each of your buckets and objects using an access control list (ACL).
  * Versioning : You can use versioning to keep multiple versions of an object in the same bucket.
  * Operations : Common operations
    * Create a bucket
    * Write an object
    * Read an object
    * Delete an object
    * List keys

## Amazon S3 application programming interfaces (API)

* The Amazon S3 architecture is designed to be programming language-neutral, using AWS Supported interfaces to store and retrieve objects.
* Amazon S3 provides a REST and a SOAP interface. 

## The REST interface

* The REST API is an HTTP interface to Amazon S3.
* Using REST, you use standard HTTP requests to create, fetch, and delete buckets and objects.
* You can use any toolkit that supports HTTP to use the REST API.
* You can even use a browser to fetch objects, as long as they are anonymously readable.

## The SOAP interface

* The SOAP API provides a SOAP 1.1 interface using document literal encoding.
