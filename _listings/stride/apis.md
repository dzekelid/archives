---
name: Stride
x-slug: stride
description: Stride is a cloud-based team business communication and collaboration
  tool, launched by Atlassian to replace the cloud-based version of HipChat. Stride
  software is available to download onto computers running Windows, Mac or Linux,
  as well as Android, iOS smartphones, and tablets
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/atlassian-stride-logo.jpg
x-kinRank: "8"
x-alexaRank: "0"
tags: Archives
created: "2018-06-17"
modified: "2018-06-17"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/archives/master/_listings/stride/apis.md
specificationVersion: "0.14"
apis:
- name: Stride Archive conversation
  x-api-slug: stride
  description: Authentication required, with scope manage:conversation
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/atlassian-stride-logo.jpg
  humanURL: https://www.stride.com/
  baseURL: https://api.atlassian.com////site/{cloudId}/conversation/{conversationId}/archive
  tags: Messaging,Site, Cloud, Conversation, Conversation, Archives
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/archives/master/_listings/stride/sitecloudidconversationconversationidarchive-put-openapi.md
- name: Stride Unarchive conversation
  x-api-slug: stride
  description: Authentication required, with scope manage:conversation
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/atlassian-stride-logo.jpg
  humanURL: https://www.stride.com/
  baseURL: https://api.atlassian.com////site/{cloudId}/conversation/{conversationId}/unarchive
  tags: Messaging,Site, Cloud, Conversation, Conversation, Unarchive, Archives
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/archives/master/_listings/stride/sitecloudidconversationconversationidunarchive-put-openapi.md
- name: Stride
  x-api-slug: stride
  description: Stride is a cloud-based team business communication and collaboration
    tool, launched by Atlassian to replace the cloud-based version of HipChat. Stride
    software is available to download onto computers running Windows, Mac or Linux,
    as well as Android, iOS smartphones, and tablets
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/atlassian-stride-logo.jpg
  humanURL: https://www.stride.com/
  baseURL: https://api.atlassian.com//
  tags: Archives
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/archives/master/_listings/stride/openapi.md
x-common:
- type: x-authentication
  url: https://developer.atlassian.com/cloud/stride/security/authentication/
- type: x-blog
  url: https://blog.stride.com/
- type: x-buttons
  url: https://developer.atlassian.com/cloud/stride/blocks/stride-button/
- type: x-developer
  url: https://developer.atlassian.com/cloud/stride/
- type: x-getting-started
  url: https://developer.atlassian.com/cloud/stride/getting-started/
- type: x-pricing
  url: https://www.stride.com/pricing
- type: x-security
  url: https://developer.atlassian.com/cloud/stride/security/security-overview/
- type: x-support
  url: https://www.stride.com/help-center
- type: x-twitter
  url: https://twitter.com/atlassianstride
- type: x-website
  url: https://www.stride.com/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---