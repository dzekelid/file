---
name: Google Drive
x-slug: google-drive
description: Google Drive is a file storage and synchronization service operated by
  Google. It allows users to store files in the cloud, synchronize files across devices,
  and share files. Google Drive encompasses Google Docs, Sheets and Slides, an office
  suite that permits collaborative editing of documents, spreadsheets, presentations,
  drawings, forms, and more.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-drive-logo-new.png
x-kinRank: "9"
x-alexaRank: "0"
tags: File
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/file/master/_listings/google-drive/apis.md
specificationVersion: "0.14"
apis:
- name: Google Drive - Get Files
  x-api-slug: files-get
  description: Lists or searches files.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-drive-logo-new.png
  humanURL: https://developers.google.com/drive/
  baseURL: https://www.googleapis.com//drive/v3
  tags: Documents, Storage, Google APIs, Stack Network, Stack, Productivity, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/file/master/_listings/google-drive/files-get-openapi.md
- name: Google Drive - Create File
  x-api-slug: files-post
  description: Creates a new file.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-drive-logo-new.png
  humanURL: https://developers.google.com/drive/
  baseURL: https://www.googleapis.com//drive/v3
  tags: Documents, Storage, Google APIs, Stack Network, Stack, Productivity, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/file/master/_listings/google-drive/files-post-openapi.md
- name: Google Drive - Generate File IDs
  x-api-slug: filesgenerateids-get
  description: Generates a set of file IDs which can be provided in create requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-drive-logo-new.png
  humanURL: https://developers.google.com/drive/
  baseURL: https://www.googleapis.com//drive/v3
  tags: Documents, Storage, Google APIs, Stack Network, Stack, Productivity, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/file/master/_listings/google-drive/filesgenerateids-get-openapi.md
- name: Google Drive - Empty Trash
  x-api-slug: filestrash-delete
  description: Permanently deletes all of the user's trashed files.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-drive-logo-new.png
  humanURL: https://developers.google.com/drive/
  baseURL: https://www.googleapis.com//drive/v3
  tags: Documents, Storage, Google APIs, Stack Network, Stack, Productivity, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/file/master/_listings/google-drive/filestrash-delete-openapi.md
- name: Google Drive - Delete File
  x-api-slug: filesfileid-delete
  description: Permanently deletes a file owned by the user without moving it to the
    trash. If the file belongs to a Team Drive the user must be an organizer on the
    parent. If the target is a folder, all descendants owned by the user are also
    deleted.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-drive-logo-new.png
  humanURL: https://developers.google.com/drive/
  baseURL: https://www.googleapis.com//drive/v3
  tags: Documents, Storage, Google APIs, Stack Network, Stack, Productivity, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/file/master/_listings/google-drive/filesfileid-delete-openapi.md
- name: Google Drive - Get File
  x-api-slug: filesfileid-get
  description: Gets a file's metadata or content by ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-drive-logo-new.png
  humanURL: https://developers.google.com/drive/
  baseURL: https://www.googleapis.com//drive/v3
  tags: Documents, Storage, Google APIs, Stack Network, Stack, Productivity, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/file/master/_listings/google-drive/filesfileid-get-openapi.md
- name: Google Drive - Update File
  x-api-slug: filesfileid-patch
  description: Updates a file's metadata and/or content with patch semantics.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-drive-logo-new.png
  humanURL: https://developers.google.com/drive/
  baseURL: https://www.googleapis.com//drive/v3
  tags: Documents, Storage, Google APIs, Stack Network, Stack, Productivity, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/file/master/_listings/google-drive/filesfileid-patch-openapi.md
- name: Google Drive - Copy File
  x-api-slug: filesfileidcopy-post
  description: Creates a copy of a file and applies any requested updates with patch
    semantics.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-drive-logo-new.png
  humanURL: https://developers.google.com/drive/
  baseURL: https://www.googleapis.com//drive/v3
  tags: Documents, Storage, Google APIs, Stack Network, Stack, Productivity, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/file/master/_listings/google-drive/filesfileidcopy-post-openapi.md
- name: Google Drive - Export File
  x-api-slug: filesfileidexport-get
  description: Exports a Google Doc to the requested MIME type and returns the exported
    content.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-drive-logo-new.png
  humanURL: https://developers.google.com/drive/
  baseURL: https://www.googleapis.com//drive/v3
  tags: Documents, Storage, Google APIs, Stack Network, Stack, Productivity, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/file/master/_listings/google-drive/filesfileidexport-get-openapi.md
- name: Google Drive - Watch File
  x-api-slug: filesfileidwatch-post
  description: Subscribes to changes to a file
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-drive-logo-new.png
  humanURL: https://developers.google.com/drive/
  baseURL: https://www.googleapis.com//drive/v3
  tags: Documents, Storage, Google APIs, Stack Network, Stack, Productivity, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/file/master/_listings/google-drive/filesfileidwatch-post-openapi.md
x-common:
- type: x-api-gallery
  url: http://google.doubleclick.api.gallery.streamdata.io
- type: x-api-stack
  url: http://google.drive.stack.network
- type: x-best-practices
  url: https://developers.google.com/drive/v3/web/practices
- type: x-branding-guidelines
  url: https://developers.google.com/drive/v3/web/marketing
- type: x-change-log
  url: https://developers.google.com/drive/release-notes
- type: x-code
  url: https://developers.google.com/drive/v3/web/downloads
- type: x-documentation
  url: https://developers.google.com/drive/v3/web/about-sdk
- type: x-github
  url: https://github.com/googledrive
- type: x-issues
  url: https://code.google.com/a/google.com/p/apps-api-issues/issues/list?q=API%3DDrive
- type: x-performance
  url: https://developers.google.com/drive/v3/web/performance
- type: x-support
  url: https://developers.google.com/drive/v3/web/support
- type: x-website
  url: https://developers.google.com/drive/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---