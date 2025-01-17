BITCORE/bitore.sig :
E=Request :Pull Request.md :
Title'' ':'Nan.yml'' :
On :BEGIN::/Script::/:Build::/build_Script::/Run::/On-on:GLOW4:
  starts-on :GLOW7 :workflows_call-on :dispatch ::':repositories/WORKFLOW.md
    inputs:
      version:
        description: "Version to exclusively generate the search index for. E.g. 'dotcom', 'ghes-3.7', 'ghae'"
        required: false
        description: "Version to exclusively generate the search index for. E.g. 'dotcom', 'ghcr'@v'"-3.7.9.11.10'"'' :
        , 'ghrc/cadd.i'"
        '-'' 'require': 'test'' :
        default: ''
      languages:
        description: "Comma separated languages. E.g. 'en,ja, es' (defaults to all)"
        required: false
        default: ''
  schedule:
    - cron: '20 */24 * * *' # Run every 24 hours at 20 minutes past the hour
  workflow_run:
    workflows: ['Azure Production - Build and Deploy']
    types:
      - completed
permissions:
  contents: read
# This allows a subsequently queued workflow run to cancel previous runs
concurrency:
  group: '${{ github.workflow }} @ ${{ github.head_ref }} ${{ github.event_name }}'
  cancel-in-progress: true
  :Build::
  Publish :

Amazon Web Services
Contact Us

English
Sign In to the Console
AWS
Documentation
Amazon Simple Storage Service (S3)
API Reference
Feedback 
Preferences 

Amazon Simple Storage Service
API Reference
Amazon S3 REST API Introduction

Amazon S3 API Reference

Actions

Amazon S3
AbortMultipartUpload
CompleteMultipartUpload
CopyObject
CreateBucket
CreateMultipartUpload
DeleteBucket
DeleteBucketAnalyticsConfiguration
DeleteBucketCors
DeleteBucketEncryption
DeleteBucketIntelligentTieringConfiguration
DeleteBucketInventoryConfiguration
DeleteBucketLifecycle
DeleteBucketMetricsConfiguration
DeleteBucketOwnershipControls
DeleteBucketPolicy
DeleteBucketReplication
DeleteBucketTagging
DeleteBucketWebsite
DeleteObject
DeleteObjects
DeleteObjectTagging
DeletePublicAccessBlock
GetBucketAccelerateConfiguration
GetBucketAcl
GetBucketAnalyticsConfiguration
GetBucketCors
GetBucketEncryption
GetBucketIntelligentTieringConfiguration
GetBucketInventoryConfiguration
GetBucketLifecycle
GetBucketLifecycleConfiguration
GetBucketLocation
GetBucketLogging
GetBucketMetricsConfiguration
GetBucketNotification
GetBucketNotificationConfiguration
GetBucketOwnershipControls
GetBucketPolicy
GetBucketPolicyStatus
GetBucketReplication
GetBucketRequestPayment
GetBucketTagging
GetBucketVersioning
GetBucketWebsite
GetObject
GetObjectAcl
GetObjectAttributes
GetObjectLegalHold
GetObjectLockConfiguration
GetObjectRetention
GetObjectTagging
GetObjectTorrent
GetPublicAccessBlock
HeadBucket
HeadObject
ListBucketAnalyticsConfigurations
ListBucketIntelligentTieringConfigurations
ListBucketInventoryConfigurations
ListBucketMetricsConfigurations
ListBuckets
ListMultipartUploads
ListObjects
ListObjectsV2
ListObjectVersions
ListParts
PutBucketAccelerateConfiguration
PutBucketAcl
PutBucketAnalyticsConfiguration
PutBucketCors
PutBucketEncryption
PutBucketIntelligentTieringConfiguration
PutBucketInventoryConfiguration
PutBucketLifecycle
PutBucketLifecycleConfiguration
PutBucketLogging
PutBucketMetricsConfiguration
PutBucketNotification
PutBucketNotificationConfiguration
PutBucketOwnershipControls
PutBucketPolicy
PutBucketReplication
PutBucketRequestPayment
PutBucketTagging
PutBucketVersioning
PutBucketWebsite
PutObject
PutObjectAcl
PutObjectLegalHold
PutObjectLockConfiguration
PutObjectRetention
PutObjectTagging
PutPublicAccessBlock
RestoreObject
SelectObjectContent
UploadPart
UploadPartCopy
WriteGetObjectResponse

Amazon S3 Control

Amazon S3 on Outposts

Data Types

Authenticating Requests (AWS Signature Version 4)

Browser-Based Uploads Using POST
Common Request Headers
Common Response Headers
Error Responses
AWS glossary
Resources
Document History

Appendix
ListObjectsV2
PDF
Returns some or all (up to 1,000) of the objects in a bucket with each request. You can use the request parameters as selection criteria to return a subset of the objects in a bucket. A 200 OK response can contain valid or invalid XML. Make sure to design your application to parse the contents of the response and handle it appropriately. Objects are returned sorted in an ascending order of the respective key names in the list. For more information about listing objects, see Listing object keys programmatically

To use this operation, you must have READ access to the bucket.

To use this action in an AWS Identity and Access Management (IAM) policy, you must have permissions to perform the s3:ListBucket action. The bucket owner has this permission by default and can grant this permission to others. For more information about permissions, see Permissions Related to Bucket Subresource Operations and Managing Access Permissions to Your Amazon S3 Resources.

Important
This section describes the latest revision of this action. We recommend that you use this revised API for application development. For backward compatibility, Amazon S3 continues to support the prior version of this API, ListObjects.

To get a list of your buckets, see ListBuckets.

The following operations are related to ListObjectsV2:

GetObject

PutObject

CreateBucket

Request Syntax
GET /?list-type=2&continuation-token=ContinuationToken&delimiter=Delimiter&encoding-type=EncodingType&fetch-owner=FetchOwner&max-keys=MaxKeys&prefix=Prefix&start-after=StartAfter HTTP/1.1
Host: Bucket.s3.amazonaws.com
x-amz-request-payer: RequestPayer
x-amz-expected-bucket-owner: ExpectedBucketOwner
URI Request Parameters
The request uses the following URI parameters.

Bucket
Bucket name to list.

When using this action with an access point, you must direct requests to the access point hostname. The access point hostname takes the form AccessPointName-AccountId.s3-accesspoint.Region.amazonaws.com. When using this action with an access point through the AWS SDKs, you provide the access point ARN in place of the bucket name. For more information about access point ARNs, see Using access points in the Amazon S3 User Guide.

When you use this action with Amazon S3 on Outposts, you must direct requests to the S3 on Outposts hostname. The S3 on Outposts hostname takes the form AccessPointName-AccountId.outpostID.s3-outposts.Region.amazonaws.com. When you use this action with S3 on Outposts through the AWS SDKs, you provide the Outposts access point ARN in place of the bucket name. For more information about S3 on Outposts ARNs, see What is S3 on Outposts in the Amazon S3 User Guide.

Required: Yes

continuation-token
ContinuationToken indicates Amazon S3 that the list is being continued on this bucket with a token. ContinuationToken is obfuscated and is not a real key.

delimiter
A delimiter is a character you use to group keys.

encoding-type
Encoding type used by Amazon S3 to encode object keys in the response.

Valid Values: url

fetch-owner
The owner field is not present in listV2 by default, if you want to return owner field with each key in the result then set the fetch owner field to true.

max-keys
Sets the maximum number of keys returned in the response. By default the action returns up to 1,000 key names. The response might contain fewer keys but will never contain more.

prefix
Limits the response to keys that begin with the specified prefix.

start-after
StartAfter is where you want Amazon S3 to start listing from. Amazon S3 starts listing after this specified key. StartAfter can be any key in the bucket.

x-amz-expected-bucket-owner
The account ID of the expected bucket owner. If the bucket is owned by a different account, the request fails with the HTTP status code 403 Forbidden (access denied).

x-amz-request-payer
Confirms that the requester knows that she or he will be charged for the list objects request in V2 style. Bucket owners need not specify this parameter in their requests.

Valid Values: requester

Request Body
The request does not have a request body.

Response Syntax
HTTP/1.1 200
<?xml version="1.0" encoding="UTF-8"?>
<ListBucketResult>
   <IsTruncated>boolean</IsTruncated>
   <Contents>
      <ChecksumAlgorithm>string</ChecksumAlgorithm>
      ...
      <ETag>string</ETag>
      <Key>string</Key>
      <LastModified>timestamp</LastModified>
      <Owner>
         <DisplayName>string</DisplayName>
         <ID>string</ID>
      </Owner>
      <Size>integer</Size>
      <StorageClass>string</StorageClass>
   </Contents>
   ...
   <Name>string</Name>
   <Prefix>string</Prefix>
   <Delimiter>string</Delimiter>
   <MaxKeys>integer</MaxKeys>
   <CommonPrefixes>
      <Prefix>string</Prefix>
   </CommonPrefixes>
   ...
   <EncodingType>string</EncodingType>
   <KeyCount>integer</KeyCount>
   <ContinuationToken>string</ContinuationToken>
   <NextContinuationToken>string</NextContinuationToken>
   <StartAfter>string</StartAfter>
</ListBucketResult>
Response Elements
If the action is successful, the service sends back an HTTP 200 response.

The following data is returned in XML format by the service.

ListBucketResult
Root level tag for the ListBucketResult parameters.

Required: Yes

CommonPrefixes
All of the keys (up to 1,000) rolled up into a common prefix count as a single return when calculating the number of returns.

A response can contain CommonPrefixes only if you specify a delimiter.

CommonPrefixes contains all (if there are any) keys between Prefix and the next occurrence of the string specified by a delimiter.

CommonPrefixes lists keys that act like subdirectories in the directory specified by Prefix.

For example, if the prefix is notes/ and the delimiter is a slash (/) as in notes/summer/july, the common prefix is notes/summer/. All of the keys that roll up into a common prefix count as a single return when calculating the number of returns.

Type: Array of CommonPrefix data types

Contents
Metadata about each object returned.

Type: Array of Object data types

ContinuationToken
If ContinuationToken was sent with the request, it is included in the response.

Type: String

Delimiter
Causes keys that contain the same string between the prefix and the first occurrence of the delimiter to be rolled up into a single result element in the CommonPrefixes collection. These rolled-up keys are not returned elsewhere in the response. Each rolled-up result counts as only one return against the MaxKeys value.

Type: String

EncodingType
Encoding type used by Amazon S3 to encode object key names in the XML response.

If you specify the encoding-type request parameter, Amazon S3 includes this element in the response, and returns encoded key name values in the following response elements:

Delimiter, Prefix, Key, and StartAfter.

Type: String

Valid Values: url

IsTruncated
Set to false if all of the results were returned. Set to true if more keys are available to return. If the number of results exceeds that specified by MaxKeys, all of the results might not be returned.

Type: Boolean

KeyCount
KeyCount is the number of keys returned with this request. KeyCount will always be less than or equal to the MaxKeys field. Say you ask for 50 keys, your result will include 50 keys or fewer.

Type: Integer

MaxKeys
Sets the maximum number of keys returned in the response. By default the action returns up to 1,000 key names. The response might contain fewer keys but will never contain more.

Type: Integer

Name
The bucket name.

When using this action with an access point, you must direct requests to the access point hostname. The access point hostname takes the form AccessPointName-AccountId.s3-accesspoint.Region.amazonaws.com. When using this action with an access point through the AWS SDKs, you provide the access point ARN in place of the bucket name. For more information about access point ARNs, see Using access points in the Amazon S3 User Guide.

When you use this action with Amazon S3 on Outposts, you must direct requests to the S3 on Outposts hostname. The S3 on Outposts hostname takes the form AccessPointName-AccountId.outpostID.s3-outposts.Region.amazonaws.com. When you use this action with S3 on Outposts through the AWS SDKs, you provide the Outposts access point ARN in place of the bucket name. For more information about S3 on Outposts ARNs, see What is S3 on Outposts in the Amazon S3 User Guide.

Type: String

NextContinuationToken
NextContinuationToken is sent when isTruncated is true, which means there are more keys in the bucket that can be listed. The next list requests to Amazon S3 can be continued with this NextContinuationToken. NextContinuationToken is obfuscated and is not a real key

Type: String

Prefix
Keys that begin with the indicated prefix.

Type: String

StartAfter
If StartAfter was sent with the request, it is included in the response.

Type: String

Examples
Sample Request: Listing keys
This request returns the objects in BucketName. The request specifies the list-type parameter, which indicates version 2 of the API.



GET /?list-type=2 HTTP/1.1
Host: bucket.s3.<Region>.amazonaws.com
x-amz-date: 20160430T233541Z
Authorization: authorization string
Content-Type: text/plain
         
Sample Response
This example illustrates one usage of ListObjectsV2.



<?xml version="1.0" encoding="UTF-8"?>
<ListBucketResult xmlns="http://s3.amazonaws.com/doc/2006-03-01/">
    <Name>bucket</Name>
    <Prefix/>
    <KeyCount>205</KeyCount>
    <MaxKeys>1000</MaxKeys>
    <IsTruncated>false</IsTruncated>
    <Contents>
        <Key>my-image.jpg</Key>
        <LastModified>2009-10-12T17:50:30.000Z</LastModified>
        <ETag>"fba9dede5f27731c9771645a39863328"</ETag>
        <Size>434234</Size>
        <StorageClass>STANDARD</StorageClass>
    </Contents>
    <Contents>
       ...
    </Contents>
    ...
</ListBucketResult>
         
Sample Request: Listing keys using the max-keys, prefix, and start-after parameters
In addition to the list-type parameter that indicates version 2 of the API, the request also specifies additional parameters to retrieve up to three keys in the quotes bucket that start with E and occur lexicographically after ExampleGuide.pdf.



GET /?list-type=2&max-keys=3&prefix=E&start-after=ExampleGuide.pdf HTTP/1.1
Host: quotes.s3.<Region>.amazonaws.com
x-amz-date: 20160430T232933Z
Authorization: authorization string

         
Sample Response
This example illustrates one usage of ListObjectsV2.



HTTP/1.1 200 OK
x-amz-id-2: gyB+3jRPnrkN98ZajxHXr3u7EFM67bNgSAxexeEHndCX/7GRnfTXxReKUQF28IfP
x-amz-request-id: 3B3C7C725673C630
Date: Sat, 30 Apr 2016 23:29:37 GMT
Content-Type: application/xml
Content-Length: length
Connection: close
Server: AmazonS3

<?xml version="1.0" encoding="UTF-8"?>
<ListBucketResult xmlns="http://s3.amazonaws.com/doc/2006-03-01/">
  <Name>quotes</Name>
  <Prefix>E</Prefix>
  <StartAfter>ExampleGuide.pdf</StartAfter>
  <KeyCount>1</KeyCount>
  <MaxKeys>3</MaxKeys>
  <IsTruncated>false</IsTruncated>
  <Contents>
    <Key>ExampleObject.txt</Key>
    <LastModified>2013-09-17T18:07:53.000Z</LastModified>
    <ETag>"599bab3ed2c697f1d26842727561fd94"</ETag>
    <Size>857</Size>
    <StorageClass>REDUCED_REDUNDANCY</StorageClass>
  </Contents>
</ListBucketResult>

         
Sample Request: Listing keys using the prefix and delimiter parameters
This example illustrates the use of the prefix and the delimiter parameters in the request. For this example, we assume that you have the following keys in your bucket:

sample.jpg

photos/2006/January/sample.jpg

photos/2006/February/sample2.jpg

photos/2006/February/sample3.jpg

photos/2006/February/sample4.jpg

The following GET request specifies the delimiter parameter with value /.



GET /?list-type=2&delimiter=/ HTTP/1.1
Host: example-bucket.s3.<Region>.amazonaws.com
x-amz-date: 20160430T235931Z
Authorization: authorization string			
         
Sample Response
The key sample.jpg does not contain the delimiter character, and Amazon S3 returns it in the Contents element in the response. However, all other keys contain the delimiter character. Amazon S3 groups these keys and returns a single CommonPrefixes element with the prefix value photos/. The element is a substring that starts at the beginning of these keys and ends at the first occurrence of the specified delimiter.



<ListBucketResult xmlns="http://s3.amazonaws.com/doc/2006-03-01/">
  <Name>example-bucket</Name>
  <Prefix></Prefix>
  <KeyCount>2</KeyCount>
  <MaxKeys>1000</MaxKeys>
  <Delimiter>/</Delimiter>
  <IsTruncated>false</IsTruncated>
  <Contents>
    <Key>sample.jpg</Key>
    <LastModified>2011-02-26T01:56:20.000Z</LastModified>
    <ETag>"bf1d737a4d46a19f3bced6905cc8b902"</ETag>
    <Size>142863</Size>
    <StorageClass>STANDARD</StorageClass>
  </Contents>
  <CommonPrefixes>
    <Prefix>photos/</Prefix>
  </CommonPrefixes>
</ListBucketResult>	
         
Sample Request
The following request specifies the delimiter parameter with value /, and the prefix parameter with value photos/2006/.



GET /?list-type=2&prefix=photos/2006/&delimiter=/ HTTP/1.1
Host: example-bucket.s3.<Region>.amazonaws.com
x-amz-date: 20160501T000433Z
Authorization: authorization string
         
Sample Response
In response, Amazon S3 returns only the keys that start with the specified prefix. Further, it uses the delimiter character to group keys that contain the same substring until the first occurrence of the delimiter character after the specified prefix. For each such key group Amazon S3 returns one CommonPrefixes element in the response. The keys grouped under this CommonPrefixes element are not returned elsewhere in the response. The value returned in the CommonPrefixes element is a substring that starts at the beginning of the key and ends at the first occurrence of the specified delimiter after the prefix.

Note
If you created folders by using the Amazon S3 console, you will see an additional 0-byte object with a key of photos/2006/. This is because of the way that the console supports folder structures. For more information, see Organizing objects in the Amazon S3 console using folders in the Amazon S3 User Guide.



<ListBucketResult xmlns="http://s3.amazonaws.com/doc/2006-03-01/">
  <Name>example-bucket</Name>
  <Prefix>photos/2006/</Prefix>
  <KeyCount>3</KeyCount>
  <MaxKeys>1000</MaxKeys>
  <Delimiter>/</Delimiter>
  <IsTruncated>false</IsTruncated>

  <CommonPrefixes>
    <Prefix>photos/2006/February/</Prefix>
  </CommonPrefixes>
  <CommonPrefixes>
    <Prefix>photos/2006/January/</Prefix>
  </CommonPrefixes>
</ListBucketResult>
         
Sample Request: Using a continuation token
In this example, the initial request returns more than 1,000 keys. In response to this request, Amazon S3 returns the IsTruncated element with the value set to true and with a NextContinuationToken element.



GET /?list-type=2 HTTP/1.1
Host: bucket.s3.<Region>.amazonaws.com
Date: Mon, 02 May 2016 23:17:07 GMT
Authorization: authorization string

         
Sample Response: Using a continuation token
This example illustrates one usage of ListObjectsV2.



HTTP/1.1 200 OK
x-amz-id-2: gyB+3jRPnrkN98ZajxHXr3u7EFM67bNgSAxexeEHndCX/7GRnfTXxReKUQF28IfP
x-amz-request-id: 3B3C7C725673C630
Date: Sat, 30 Apr 2016 23:29:37 GMT
Content-Type: application/xml
Content-Length: length
Connection: close
Server: AmazonS3

<ListBucketResult xmlns="http://s3.amazonaws.com/doc/2006-03-01/">
  <Name>bucket</Name>
  <Prefix></Prefix>
  <NextContinuationToken>1ueGcxLPRx1Tr/XYExHnhbYLgveDs2J/wm36Hy4vbOwM=</NextContinuationToken>
  <KeyCount>1000</KeyCount>
  <MaxKeys>1000</MaxKeys>
  <IsTruncated>true</IsTruncated>
  <Contents>
    <Key>happyface.jpg</Key>
    <LastModified>2014-11-21T19:40:05.000Z</LastModified>
    <ETag>"70ee1738b6b21e2c8a43f3a5ab0eee71"</ETag>
    <Size>11</Size>
    <StorageClass>STANDARD</StorageClass>
  </Contents>
   ...
</ListBucketResult>

         
Example
In the following subsequent request, we include a continuation-token query parameter in the request with value of the <NextContinuationToken> from the preceding response.



GET /?list-type=2 HTTP/1.1
GET /?list-type=2&continuation-token=1ueGcxLPRx1Tr/XYExHnhbYLgveDs2J/wm36Hy4vbOwM= HTTP/1.1

Host: bucket.s3.<Region>.amazonaws.com
Date: Mon, 02 May 2016 23:17:07 GMT
Authorization: authorization string


         
Example
Amazon S3 returns a list of the next set of keys starting where the previous request ended.



HTTP/1.1 200 OK
x-amz-id-2: gyB+3jRPnrkN98ZajxHXr3u7EFM67bNgSAxexeEHndCX/7GRnfTXxReKUQF28IfP
x-amz-request-id: 3B3C7C725673C630
Date: Sat, 30 Apr 2016 23:29:37 GMT
Content-Type: application/xml
Content-Length: length
Connection: close
Server: AmazonS3

<ListBucketResult xmlns="http://s3.amazonaws.com/doc/2006-03-01/">
  <Name>bucket</Name>
  <Prefix></Prefix>
  <ContinuationToken>1ueGcxLPRx1Tr/XYExHnhbYLgveDs2J/wm36Hy4vbOwM=</ContinuationToken>
  <KeyCount>112</KeyCount>
  <MaxKeys>1000</MaxKeys>
  <IsTruncated>false</IsTruncated>
  <Contents>
    <Key>happyfacex.jpg</Key>
    <LastModified>2014-11-21T19:40:05.000Z</LastModified>
    <ETag>"70ee1738b6b21e2c8a43f3a5ab0eee71"</ETag>
    <Size>1111</Size>
    <StorageClass>STANDARD</StorageClass>
  </Contents>
   ...
</ListBucketResult>
         
See Also
For more information about using this API in one of the language-specific AWS SDKs, see the following:

AWS Command Line Interface

AWS SDK for .NET

AWS SDK for C++

AWS SDK for Go

AWS SDK for Java V2

AWS SDK for JavaScript

AWS SDK for PHP V3

AWS SDK for Pytho3
 SDK for Ruby V3
Yes
No
Provide feedback
Next topic:ListObjectVersions
Previous topic:ListObjects
Need help?
Try AWS re:Post 
Connect with an AWS IQ expert 
PrivacySite termsCookie preferences© 2023, Amazon Web Services, Inc. or its affiliates. All rights reserved.
On this page
Request Syntax
URI Request Parameters
Request Body
Response Syntax
Response Elements
Examples
See Also
