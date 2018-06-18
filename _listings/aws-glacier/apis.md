---
name: AWS Glacier
x-slug: aws-glacier
description: Amazon Glacier is a secure, durable, and extremely low-cost cloud storage
  service for data archiving and long-term backup. Customers can reliably store large
  or small amounts of data for as little as $0.004 per gigabyte per month, a significant
  savings compared to on-premises solutions. To keep costs low yet suitable for varying
  retrieval needs, Amazon Glacier provides three options for access to archives, from
  a few minutes to several hours.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AmazonGlacier.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Archives
created: "2018-06-17"
modified: "2018-06-17"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/archives/master/_listings/aws-glacier/apis.md
specificationVersion: "0.14"
apis:
- name: Amazon Glacier API Upload  Archive
  x-api-slug: amazon-glacier-api
  description: "DescriptionThis operation adds an archive to a vault. For a successful
    upload, your data is durably\n\t\t\tpersisted. In response, Amazon Glacier returns
    the archive ID in the\n\t\t\t\tx-amz-archive-id header of the response. You should
    save the archive ID\n\t\t\treturned so that you can access the archive later.
    You must provide a SHA256 tree hash of the data you are uploading. For information
    about\n\t\t\tcomputing a SHA256 tree hash, see Computing Checksums. When uploading
    an archive, you can optionally specify an archive description of up to 1,024\n\t\t\tprintable
    ASCII characters. Amazon Glacier returns the archive description when you\n\t\t\teither
    retrieve the archive or get the vault inventory. Amazon Glacier does not interpret
    the\n\t\t\tdescription in any way. An archive description does not need to be
    unique. You cannot\n\t\t\tuse the description to retrieve or sort the archive
    list. Except for the optional archive description, Amazon Glacier does not support
    any\n\t\t\tadditional metadata for the archives. The archive ID is an opaque sequence
    of characters\n\t\t\tfrom which you cannot infer any meaning about the archive.
    So you might maintain\n\t\t\tmetadata about the archives on the client-side. For
    more information, see \n\t\t\tWorking with Archives in Amazon Glacier.Archives
    are immutable. After you upload an archive, you cannot edit the archive or its\n\t\t\tdescription.
    RequestsTo upload an archive, you use the HTTP POST method and scope the request
    to the\n\t\t\t\tarchives subresource of the vault in which you want to save the\n\t\t\tarchive.
    The request must include the archive payload size, checksum (SHA256 tree hash),\n\t\t\tand
    can optionally include a description of the archive."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AmazonGlacier.png
  humanURL: https://aws.amazon.com/glacier/
  baseURL: ://///{AccountId}/vaults/{VaultName}/archives
  tags: Archives
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/archives/master/_listings/aws-glacier/accountidvaultsvaultnamearchives-post-openapi.md
- name: Amazon Glacier API Delete  Archive
  x-api-slug: amazon-glacier-api
  description: "DescriptionThis operation deletes an archive from a vault. You can
    delete one archive at a time from a vault. \n\t\t\tTo delete the archive you must
    provide its archive ID in the delete request. \n\t\t\tYou can get the archive
    ID by downloading the vault inventory for the vault that contains the archive.
    \n\t\t\tFor more information about downloading the vault inventory, \n\t\t\tsee
    Downloading a Vault Inventory in Amazon Glacier.After you delete an archive, you
    might still\n\t\t\tbe able to make a successful request to initiate a job to retrieve
    the deleted archive,\n\t\t\tbut the archive retrieval job will fail. Archive retrievals
    that are in progress for an archive ID when you delete the\n\t\t\tarchive might
    or might not succeed according to the following scenarios:\n\t\t\tIf the archive
    retrieval job is actively preparing the data for download when Amazon Glacier\n\t\t\t\t\t\treceives
    the delete archive request, the archival retrieval\toperation might fail. If the
    archive retrieval job has successfully prepared the archive for download when\n\t\t\t\t\t\tAmazon
    Glacier receives the delete archive request, you will be able to\n\t\t\t\t\t\tdownload
    the output. \n\t\tFor more information about archive retrieval, see \n\t\t\tDownloading
    an Archive in Amazon Glacier. This operation is idempotent. Attempting\n\t\t\tto
    delete an already-deleted archive does not result in an error. RequestsTo delete
    an archive you send a DELETE request to the archive resource\n\t\t\tURI."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AmazonGlacier.png
  humanURL: https://aws.amazon.com/glacier/
  baseURL: ://///{AccountId}/vaults/{VaultName}/archives/{ArchiveID}
  tags: Archives
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/archives/master/_listings/aws-glacier/accountidvaultsvaultnamearchivesarchiveid-delete-openapi.md
- name: Amazon Glacier API
  x-api-slug: amazon-glacier-api
  description: Amazon Glacier is a secure, durable, and extremely low-cost cloud storage
    service for data archiving and long-term backup. Customers can reliably store
    large or small amounts of data for as little as $0.004 per gigabyte per month,
    a significant savings compared to on-premises solutions. To keep costs low yet
    suitable for varying retrieval needs, Amazon Glacier provides three options for
    access to archives, from a few minutes to several hours.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Storage-Content-Delivery_AmazonGlacier.png
  humanURL: https://aws.amazon.com/glacier/
  baseURL: :///
  tags: Archives
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/archives/master/_listings/aws-glacier/openapi.md
x-common:
- type: x-change-log
  url: http://aws.amazon.com/releasenotes/Amazon-Glacier/
- type: x-documentation
  url: http://docs.aws.amazon.com/amazonglacier/latest/dev/amazon-glacier-api.html
- type: x-faq
  url: https://aws.amazon.com/glacier/faqs/
- type: x-forum
  url: https://forums.aws.amazon.com/forum.jspa?forumID=140
- type: x-getting-started
  url: https://aws.amazon.com/glacier/getting-started/
- type: x-pricing
  url: https://aws.amazon.com/glacier/pricing/
- type: x-website
  url: https://aws.amazon.com/glacier/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---