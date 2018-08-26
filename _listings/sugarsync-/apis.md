---
name: SugarSync
x-slug: sugarsync-
description: SugarSync is a cloud file sharing, file sync and online backup service
  that is simple, powerful and easy to use. Unlike Dropbox, SugarSync enables you
  to back up your existing folder structure. Try it for FREE for 30 days and get started
  today!
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/488-sugarsync-.jpg
x-kinRank: "8"
x-alexaRank: "64898"
tags: File
created: "2018-08-25"
modified: "2018-08-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/file/master/_listings/sugarsync-/apis.md
specificationVersion: "0.14"
apis:
- name: Sugar Sync  API - Retrieving File Data
  x-api-slug: file-get
  description: To retrieve file data, an application submits an HTTP GET request to
    then          file data resource that represents the data for the file.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/488-sugarsync-.jpg
  humanURL: http://sugarsync.com
  baseURL: https://api.sugarsync.com//
  tags: Cloud, Storage, Storage, File, Storage, Target, Getting Started Example, Stack
    Network, Technology, Mobile, SaaS, internet, Relative Data, Service API, Relative
    StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/file/master/_listings/sugarsync-/file-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/file/master/_listings/sugarsync-/file-get-openapi.md
- name: Sugar Sync  API - Uploading File Data
  x-api-slug: file-put
  description: An application can upload data to a file by issuing an HTTP PUT request
    to thenfile data resource that represents the data for the file.n
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/488-sugarsync-.jpg
  humanURL: http://sugarsync.com
  baseURL: https://api.sugarsync.com//
  tags: Cloud, Storage, Storage, File, Storage, Target, Getting Started Example, Stack
    Network, Technology, Mobile, SaaS, internet, Relative Data, Service API, Relative
    StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/file/master/_listings/sugarsync-/file-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/file/master/_listings/sugarsync-/file-put-openapi.md
- name: Sugar Sync  API - Deleting a File
  x-api-slug: file-delete
  description: An application can permanently delete a file by issuing an HTTP DELETE
    request to the URL of thenfile resource.nIts a good idea to precede DELETE requests
    like this with a caution note in your applications user interface.n
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/488-sugarsync-.jpg
  humanURL: http://sugarsync.com
  baseURL: https://api.sugarsync.com//
  tags: Cloud, Storage, Storage, File, Storage, Target, Getting Started Example, Stack
    Network, Technology, Mobile, SaaS, internet, Relative Data, Service API, Relative
    StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/file/master/_listings/sugarsync-/file-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/file/master/_listings/sugarsync-/file-delete-openapi.md
- name: Sugar Sync  API - Retrieving File Information
  x-api-slug: file-get
  description: To retrieve information about a file, an application submits an HTTP
    GET request to then          file resource that represents the file.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/488-sugarsync-.jpg
  humanURL: http://sugarsync.com
  baseURL: https://api.sugarsync.com//
  tags: Cloud, Storage, Storage, File, Storage, Target, Getting Started Example, Stack
    Network, Technology, Mobile, SaaS, internet, Relative Data, Service API, Relative
    StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/file/master/_listings/sugarsync-/file-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/file/master/_listings/sugarsync-/file-get-openapi.md
- name: Sugar Sync  API - Creating a New File Version
  x-api-slug: file-post
  description: nAn application can create a new version of a file by submitting an
    HTTP POST request to the URL that represents the version history. The version
    history URL is returned in the &lt;versions&gt; element whenn retrieving information
    about a file.n
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/488-sugarsync-.jpg
  humanURL: http://sugarsync.com
  baseURL: https://api.sugarsync.com//
  tags: Cloud, Storage, Storage, File, Storage, Target, Getting Started Example, Stack
    Network, Technology, Mobile, SaaS, internet, Relative Data, Service API, Relative
    StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/file/master/_listings/sugarsync-/file-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/file/master/_listings/sugarsync-/file-post-openapi.md
- name: Sugar Sync  API - Updating File Information
  x-api-slug: file-put
  description: An application can update various attributes of a file by issuing an
    HTTP PUT request to the URL thatnrepresents the file resource. In addition, the
    app needs to provide as input, XML that identifies the new attribute values for
    the file. Upon receiving the PUT request, the SugarSync service examines the input
    and updates any of the attributes that have been modified.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/488-sugarsync-.jpg
  humanURL: http://sugarsync.com
  baseURL: https://api.sugarsync.com//
  tags: Cloud, Storage, Storage, File, Storage, Target, Getting Started Example, Stack
    Network, Technology, Mobile, SaaS, internet, Relative Data, Service API, Relative
    StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/file/master/_listings/sugarsync-/file-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/file/master/_listings/sugarsync-/file-put-openapi.md
x-common:
- type: x-api-gallery
  url: http://stripe.api.gallery.streamdata.io
- type: x-api-stack
  url: http://sugarsync..stack.network
- type: x-application-gallery
  url: https://www.sugarsync.com/partners/
- type: x-base
  url: https://api.sugarsync.com
- type: x-best-practices
  url: https://www.sugarsync.com/dev/best-practices.html
- type: x-blog
  url: http://www.sugarsync.com/blog
- type: x-blog-rss
  url: http://blog.sugarsync.com/blog/feed
- type: x-crunchbase
  url: https://crunchbase.com/organization/sugarsync
- type: x-crunchbase
  url: http://www.crunchbase.com/company/sugarsync
- type: x-developer
  url: https://www.sugarsync.com/developer
- type: x-forum
  url: https://groups.google.com/a/developers.sugarsync.com/forum/#!forum/platform-api/join
- type: x-getting-started
  url: https://www.sugarsync.com/dev/getting-started.html
- type: x-glossary
  url: https://www.sugarsync.com/dev/glossary.html
- type: x-linkedin
  url: https://www.linkedin.com/company/sugarsync
- type: x-pricing
  url: https://www.sugarsync.com/
- type: x-selfservice-registration
  url: https://www.sugarsync.com/developer/signup
- type: x-terms-of-service
  url: https://www.sugarsync.com/dev/terms.html
- type: x-twitter
  url: https://twitter.com/SugarSync
- type: x-website
  url: http://sugarsync.com
- type: x-website
  url: http://www.sugarsync.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---