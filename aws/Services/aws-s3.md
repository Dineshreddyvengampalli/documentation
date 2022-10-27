# AWS S3 - simple storage service
S3 is the simple storage service by amazon web services.It is called as s3 bucket that can store the data in the form of objects.Each object has its keyname (used to describe the metadata of the file).The buckets and objects are stored private and they can be accessed only if the user grants the perticular permissions and policies.

## Buckets
Buckets are for storing the objects.Every object is stored in the bucket.Each account can be able to create 100 byckets,further on request can create more than 100 buckets.To create the bucket , one should specify the name of the bucket and the region and should follow the naming rules. Once the bucket is created , it is not possible to rename the bucket and change the location.

For suppose if the object : myname.jpg is stored in the bucket named : MY-COLLECTION with the location as : ap-south then it can be accessed by using the the link `https://MY-COLLECTION.s3.ap-south-1.amazonaws.com/myname.jpg`.

## Objects
Objects are the basic entities that can be stored in the buckets.These objects contain object-data and meta-data.Meta-data is the collection of all the data about the object.This meta-data contains some of the default values and values by the user custom data. These objects are identified by the key / version id if it contains multiple versions.

## Keys
Every object in the bucket shall contain one key.It is also reffered as the name of the object.The object is uniquely identified by : bucket,key and version.

## Bucket policy
Bucket policies use Json based structure to grant permissions to the specific ARNs to provide access.These policies can control over the accessibility of the objects and the buckets.

## Access control lists
With ACLs one can be able to setup permissions / authorize the users to access the specific bucket and object . These are usefull if you want to set permissions for individual object in the bucket.By default, the creator of the bucket adds in ACLs.It is not recommended to turn on ACL by aws.

## Creation of S3 bucket
To create s3 bucket one will have to create / authorized account of AWS.There are developer mode in creating s3 bucket through code and via console.Here are the steps to create s3 bucket through console:
* Login to aws account 
* Navigate to "[https://console.aws.amazon.com/s3/]"
* Choose create bucket.
* Enter the bucket-name
* Choose the region
* Choose create bucket

## Uploading object to the bucket
* Choose the perticular bucket to upload the object
* On the objects tab , choose upload
* Choose add files
* choose open and choose upload

## Downloading the object from S3 bucket
* Choose the perticular bucket to download the object from
* Select the needed object and choose download

