---
name: Box
x-slug: box
description: Box is changing how you manage content across your business from simple
  file sharing to building custom apps.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
x-kinRank: "9"
x-alexaRank: "445"
tags: Documents
created: "2018-08-26"
modified: "2018-08-26"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/apis.md
specificationVersion: "0.14"
apis:
- name: Box - Get File's Info, Get Embed Link
  x-api-slug: filesfile-id-get
  description: Used to retrieve the metadata about a file.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files, Collaboration, Sharing, Storage, Storage, Stack Network, Stack, Productivity,
    SaaS, Technology, Enterprise, API Provider, Profiles, Publish, Service API, Relative
    Data, Relative StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/filesfile-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/filesfile-id-get-openapi.md
- name: Box - Delete File
  x-api-slug: filesfile-id-delete
  description: Discards a file to the trash. The etag of the file can be included
    as an ???If-Match??? header to prevent race conditions.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files, Collaboration, Sharing, Storage, Storage, Stack Network, Stack, Productivity,
    SaaS, Technology, Enterprise, API Provider, Profiles, Publish, Service API, Relative
    Data, Relative StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/filesfile-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/filesfile-id-delete-openapi.md
- name: Box - Download File
  x-api-slug: filesfile-idcontent-get
  description: Retrieves the actual data of the file. An optional version parameter
    can be set to download a previous version of the file.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files, Collaboration, Sharing, Storage, Storage, Stack Network, Stack, Productivity,
    SaaS, Technology, Enterprise, API Provider, Profiles, Publish, Service API, Relative
    Data, Relative StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/filesfile-idcontent-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/filesfile-idcontent-get-openapi.md
- name: Box - View Versions
  x-api-slug: filesfile-idversions-get
  description: If there are previous versions of this file, this method can be used
    to retrieve information about the older versions. (Versions are only tracked for
    Box users with premium accounts.)
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files, Collaboration, Sharing, Storage, Storage, Stack Network, Stack, Productivity,
    SaaS, Technology, Enterprise, API Provider, Profiles, Publish, Service API, Relative
    Data, Relative StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/filesfile-idversions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/filesfile-idversions-get-openapi.md
- name: Box - Delete Old Version
  x-api-slug: filesfile-idversionsversion-id-delete
  description: Discards a specific file version to the trash. (Depending on the enterprise
    settings for this user, the item will either be actually deleted from Box or moved
    to the trash.)
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files, Collaboration, Sharing, Storage, Storage, Stack Network, Stack, Productivity,
    SaaS, Technology, Enterprise, API Provider, Profiles, Publish, Service API, Relative
    Data, Relative StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/filesfile-idversionsversion-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/filesfile-idversionsversion-id-delete-openapi.md
- name: Box - Get Thumbnail
  x-api-slug: filesfile-idthumbnail-extension-get
  description: Retrieves a thumbnail, or smaller image representation, of this file.
    Sizes of 32x32,64x64, 128x128, and 256x256 can be returned in the .png format
    and sizes of 32x32, 94x94, 160x160, and 320x320 can be returned in the .jpg format.
    Thumbnails can be generated for the image and video file formats listed here.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files, Collaboration, Sharing, Storage, Storage, Stack Network, Stack, Productivity,
    SaaS, Technology, Enterprise, API Provider, Profiles, Publish, Service API, Relative
    Data, Relative StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/filesfile-idthumbnail-extension-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/filesfile-idthumbnail-extension-get-openapi.md
- name: Box - Get Trashed File
  x-api-slug: filesfile-idtrash-get
  description: Retrieves an item that has been moved to the trash.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files, Collaboration, Sharing, Storage, Storage, Stack Network, Stack, Productivity,
    SaaS, Technology, Enterprise, API Provider, Profiles, Publish, Service API, Relative
    Data, Relative StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/filesfile-idtrash-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/filesfile-idtrash-get-openapi.md
- name: Box - Permanently Delete
  x-api-slug: filesfile-idtrash-delete
  description: Permanently deletes an item that is in the trash. The item will no
    longer exist in Box. This action cannot be undone.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files, Collaboration, Sharing, Storage, Storage, Stack Network, Stack, Productivity,
    SaaS, Technology, Enterprise, API Provider, Profiles, Publish, Service API, Relative
    Data, Relative StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/filesfile-idtrash-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/filesfile-idtrash-delete-openapi.md
- name: Box - Get File's Comments
  x-api-slug: filesfile-idcomments-get
  description: Retrieves the comments on a particular file, if any exist.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files, Collaboration, Sharing, Storage, Storage, Stack Network, Stack, Productivity,
    SaaS, Technology, Enterprise, API Provider, Profiles, Publish, Service API, Relative
    Data, Relative StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/filesfile-idcomments-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/filesfile-idcomments-get-openapi.md
- name: Box - Get File's Collaborations
  x-api-slug: filesfile-idcollaborations-get
  description: Use this to get a list of all the collaborations on a file
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files, Collaboration, Sharing, Storage, Storage, Stack Network, Stack, Productivity,
    SaaS, Technology, Enterprise, API Provider, Profiles, Publish, Service API, Relative
    Data, Relative StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/filesfile-idcollaborations-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/filesfile-idcollaborations-get-openapi.md
- name: Box - Get File's Tasks
  x-api-slug: filesfile-idtasks-get
  description: Retrieves all of the tasks for given file.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files, Collaboration, Sharing, Storage, Storage, Stack Network, Stack, Productivity,
    SaaS, Technology, Enterprise, API Provider, Profiles, Publish, Service API, Relative
    Data, Relative StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/filesfile-idtasks-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/filesfile-idtasks-get-openapi.md
- name: Box - Get Folder's Info
  x-api-slug: foldersfolder-id-get
  description: Retrieves the full metadata about a folder, including information about
    when it was last updated as well as the files and folders contained in it. The
    root folder of a Box account is always represented by the id ???0???.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files, Collaboration, Sharing, Storage, Storage, Stack Network, Stack, Productivity,
    SaaS, Technology, Enterprise, API Provider, Profiles, Publish, Service API, Relative
    Data, Relative StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/foldersfolder-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/foldersfolder-id-get-openapi.md
- name: Box - Delete Folder
  x-api-slug: foldersfolder-id-delete
  description: Used to delete a folder. A recursive parameter must be included in
    order to delete folders that have items inside of them. An optional If-Match header
    can be included to ensure that client only deletes the folder if it knows about
    the latest version.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files, Collaboration, Sharing, Storage, Storage, Stack Network, Stack, Productivity,
    SaaS, Technology, Enterprise, API Provider, Profiles, Publish, Service API, Relative
    Data, Relative StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/foldersfolder-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/foldersfolder-id-delete-openapi.md
- name: Box - Get Folder???s Items
  x-api-slug: foldersfolder-iditems-get
  description: Retrieves the files and/or folders contained within this folder without
    any other metadata about the folder. Any attribute in the full files or folders
    objects can be passed in with the fields parameter to get specific attributes,
    and only those specific attributes back; otherwise, the mini format is returned
    for each item by default. Multiple attributes can be passed in separated by commas
    e.g. fields=name,created_at. Paginated results can be retrieved using the limit
    and offset parameters.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files, Collaboration, Sharing, Storage, Storage, Stack Network, Stack, Productivity,
    SaaS, Technology, Enterprise, API Provider, Profiles, Publish, Service API, Relative
    Data, Relative StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/foldersfolder-iditems-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/foldersfolder-iditems-get-openapi.md
- name: Box - Get Folder Collaborations
  x-api-slug: foldersfolder-idcollaborations-get
  description: Use this to get a list of all the collaborations on a folder i.e. all
    of the users that have access to that folder.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files, Collaboration, Sharing, Storage, Storage, Stack Network, Stack, Productivity,
    SaaS, Technology, Enterprise, API Provider, Profiles, Publish, Service API, Relative
    Data, Relative StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/foldersfolder-idcollaborations-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/foldersfolder-idcollaborations-get-openapi.md
- name: Box - Get Trashed Folder
  x-api-slug: foldersfolder-idtrash-get
  description: Retrieves an folder that has been moved to the trash.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files, Collaboration, Sharing, Storage, Storage, Stack Network, Stack, Productivity,
    SaaS, Technology, Enterprise, API Provider, Profiles, Publish, Service API, Relative
    Data, Relative StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/foldersfolder-idtrash-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/foldersfolder-idtrash-get-openapi.md
- name: Box - Permanently Delete
  x-api-slug: foldersfolder-idtrash-delete
  description: Permanently deletes an folder that is in the trash. The item will no
    longer exist in Box. This action cannot be undone.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files, Collaboration, Sharing, Storage, Storage, Stack Network, Stack, Productivity,
    SaaS, Technology, Enterprise, API Provider, Profiles, Publish, Service API, Relative
    Data, Relative StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/foldersfolder-idtrash-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/foldersfolder-idtrash-delete-openapi.md
- name: Box - Get Trashed Items
  x-api-slug: folderstrashitems-get
  description: Retrieves the files and/or folders that have been moved to the trash.
    Any attribute in the full files or folders objects can be passed in with the fields
    parameter to get specific attributes, and only those specific attributes back;
    otherwise, the mini format is returned for each item by default. Multiple attributes
    can be passed in separated by commas e.g. fields=name,created_at. Paginated results
    can be retrieved using the limit and offset parameters.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files, Collaboration, Sharing, Storage, Storage, Stack Network, Stack, Productivity,
    SaaS, Technology, Enterprise, API Provider, Profiles, Publish, Service API, Relative
    Data, Relative StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/folderstrashitems-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/folderstrashitems-get-openapi.md
- name: Box - Get Watermark on File
  x-api-slug: filesfile-idwatermark-get
  description: Used to retrieve the watermark for a corresponding Box file.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files, Collaboration, Sharing, Storage, Storage, Stack Network, Stack, Productivity,
    SaaS, Technology, Enterprise, API Provider, Profiles, Publish, Service API, Relative
    Data, Relative StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/filesfile-idwatermark-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/filesfile-idwatermark-get-openapi.md
- name: Box - Remove Watermark on File
  x-api-slug: filesfile-idwatermark-delete
  description: Used to remove the watermark for a corresponding Box file.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files, Collaboration, Sharing, Storage, Storage, Stack Network, Stack, Productivity,
    SaaS, Technology, Enterprise, API Provider, Profiles, Publish, Service API, Relative
    Data, Relative StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/filesfile-idwatermark-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/filesfile-idwatermark-delete-openapi.md
- name: Box - Get Watermark on Folder
  x-api-slug: foldersfolder-idwatermark-get
  description: Used to retrieve the watermark for a corresponding Box folder.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files, Collaboration, Sharing, Storage, Storage, Stack Network, Stack, Productivity,
    SaaS, Technology, Enterprise, API Provider, Profiles, Publish, Service API, Relative
    Data, Relative StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/foldersfolder-idwatermark-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/foldersfolder-idwatermark-get-openapi.md
- name: Box - Remove Watermark on Folder
  x-api-slug: foldersfolder-idwatermark-delete
  description: Used to remove the watermark for a corresponding Box Folder.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files, Collaboration, Sharing, Storage, Storage, Stack Network, Stack, Productivity,
    SaaS, Technology, Enterprise, API Provider, Profiles, Publish, Service API, Relative
    Data, Relative StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/foldersfolder-idwatermark-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/foldersfolder-idwatermark-delete-openapi.md
- name: Box - Get Web Link
  x-api-slug: web-linksweb-link-id-get
  description: Use to get information about the web link.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files, Collaboration, Sharing, Storage, Storage, Stack Network, Stack, Productivity,
    SaaS, Technology, Enterprise, API Provider, Profiles, Publish, Service API, Relative
    Data, Relative StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/web-linksweb-link-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/web-linksweb-link-id-get-openapi.md
- name: Box - Delete Web Link
  x-api-slug: web-linksweb-link-id-delete
  description: Deletes a web link and moves it to the trash
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files, Collaboration, Sharing, Storage, Storage, Stack Network, Stack, Productivity,
    SaaS, Technology, Enterprise, API Provider, Profiles, Publish, Service API, Relative
    Data, Relative StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/web-linksweb-link-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/web-linksweb-link-id-delete-openapi.md
- name: Box - Get Enterprise Metadata
  x-api-slug: metadata-templatesscope-get
  description: Used to retrieve all metadata templates within a user's enterprise.
    Currently only the enterprise scope is supported.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files, Collaboration, Sharing, Storage, Storage, Stack Network, Stack, Productivity,
    SaaS, Technology, Enterprise, API Provider, Profiles, Publish, Service API, Relative
    Data, Relative StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/metadata-templatesscope-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/metadata-templatesscope-get-openapi.md
- name: Box - Get Metadata Template
  x-api-slug: metadata-templatesscopetemplateschema-get
  description: Used to retrieve the schema for a given metadata template.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files, Collaboration, Sharing, Storage, Storage, Stack Network, Stack, Productivity,
    SaaS, Technology, Enterprise, API Provider, Profiles, Publish, Service API, Relative
    Data, Relative StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/metadata-templatesscopetemplateschema-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/metadata-templatesscopetemplateschema-get-openapi.md
- name: Box - Get all Metadata on File
  x-api-slug: filesfile-idmetadata-get
  description: Used to retrieve all metadata associated with a given file
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files, Collaboration, Sharing, Storage, Storage, Stack Network, Stack, Productivity,
    SaaS, Technology, Enterprise, API Provider, Profiles, Publish, Service API, Relative
    Data, Relative StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/filesfile-idmetadata-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/filesfile-idmetadata-get-openapi.md
- name: Box - Get Metadata on File
  x-api-slug: filesfile-idmetadatascopetemplate-get
  description: Used to retrieve the metadata template instance for a corresponding
    Box file.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files, Collaboration, Sharing, Storage, Storage, Stack Network, Stack, Productivity,
    SaaS, Technology, Enterprise, API Provider, Profiles, Publish, Service API, Relative
    Data, Relative StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/filesfile-idmetadatascopetemplate-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/filesfile-idmetadatascopetemplate-get-openapi.md
- name: Box - Delete Metadata on File
  x-api-slug: filesfile-idmetadatascopetemplate-delete
  description: Used to delete the template instance. To delete custom key:value pairs
    within a template instance, you should refer to the updating metadata section.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files, Collaboration, Sharing, Storage, Storage, Stack Network, Stack, Productivity,
    SaaS, Technology, Enterprise, API Provider, Profiles, Publish, Service API, Relative
    Data, Relative StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/filesfile-idmetadatascopetemplate-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/filesfile-idmetadatascopetemplate-delete-openapi.md
- name: Box - Get All Metadata on Folder
  x-api-slug: foldersfolder-idmetadata-get
  description: Used to retrieve all metadata associated with a given folder
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files, Collaboration, Sharing, Storage, Storage, Stack Network, Stack, Productivity,
    SaaS, Technology, Enterprise, API Provider, Profiles, Publish, Service API, Relative
    Data, Relative StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/foldersfolder-idmetadata-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/foldersfolder-idmetadata-get-openapi.md
- name: Box - Get Metadata on Folder
  x-api-slug: foldersfolder-idmetadatascopetemplate-get
  description: Used to retrieve the metadata template instance for a corresponding
    Box folder.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files, Collaboration, Sharing, Storage, Storage, Stack Network, Stack, Productivity,
    SaaS, Technology, Enterprise, API Provider, Profiles, Publish, Service API, Relative
    Data, Relative StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/foldersfolder-idmetadatascopetemplate-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/foldersfolder-idmetadatascopetemplate-get-openapi.md
- name: Box - Delete Metadata on Folder
  x-api-slug: foldersfolder-idmetadatascopetemplate-delete
  description: Used to delete the template instance. To delete custom key:value pairs
    within a template instance, you should refer to the updating metadata section.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files, Collaboration, Sharing, Storage, Storage, Stack Network, Stack, Productivity,
    SaaS, Technology, Enterprise, API Provider, Profiles, Publish, Service API, Relative
    Data, Relative StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/foldersfolder-idmetadatascopetemplate-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/foldersfolder-idmetadatascopetemplate-delete-openapi.md
- name: Box - Pending Collaborations
  x-api-slug: collaborations-get
  description: Used to retrieve all pending collaboration invites for this user.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files, Collaboration, Sharing, Storage, Storage, Stack Network, Stack, Productivity,
    SaaS, Technology, Enterprise, API Provider, Profiles, Publish, Service API, Relative
    Data, Relative StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/collaborations-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/collaborations-get-openapi.md
- name: Box - Get Collaboration
  x-api-slug: collaborationscollab-id-get
  description: Used to get information about a single collaboration. All collaborations
    for a single folder can be retrieved through GET /folders/{id}/collaborations.
    A complete list of the user???s pending collaborations can also be retrieved.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files, Collaboration, Sharing, Storage, Storage, Stack Network, Stack, Productivity,
    SaaS, Technology, Enterprise, API Provider, Profiles, Publish, Service API, Relative
    Data, Relative StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/collaborationscollab-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/collaborationscollab-id-get-openapi.md
- name: Box - Delete Collaboration
  x-api-slug: collaborationscollab-id-delete
  description: Used to delete a single collaboration.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files, Collaboration, Sharing, Storage, Storage, Stack Network, Stack, Productivity,
    SaaS, Technology, Enterprise, API Provider, Profiles, Publish, Service API, Relative
    Data, Relative StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/collaborationscollab-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/collaborationscollab-id-delete-openapi.md
- name: Box - Searching for Content
  x-api-slug: search-get
  description: The search endpoint provides a powerful way of finding items that are
    accessible by a single user or an entire enterprise. Leverage the parameters listed
    below to generate targeted advanced searches.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files, Collaboration, Sharing, Storage, Storage, Stack Network, Stack, Productivity,
    SaaS, Technology, Enterprise, API Provider, Profiles, Publish, Service API, Relative
    Data, Relative StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/search-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/search-get-openapi.md
- name: Box - Shared Items
  x-api-slug: shared-items-get
  description: |-
    Shared items are any files or folders that are represented by a shared link. Shared items are different from other API resources in that a shared resource doesn???t necessarily have to be in the account of the user accessing it. The actual shared link itself is used along with a normal access token.
    Used to retrieve the metadata about a shared item when only given a shared link. Because of varying permission for shared links, a password may be required to retrieve the shared item. Once the item has been retrieved, you can make API requests against the actual resource /files/{id} or /folders/{id} as long as the shared link and optional password are in the header.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files, Collaboration, Sharing, Storage, Storage, Stack Network, Stack, Productivity,
    SaaS, Technology, Enterprise, API Provider, Profiles, Publish, Service API, Relative
    Data, Relative StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/shared-items-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/shared-items-get-openapi.md
- name: Box - Get Collections
  x-api-slug: collections-get
  description: Retrieves the collections for the given user. Currently, only the favorites
    collection is supported.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files, Collaboration, Sharing, Storage, Storage, Stack Network, Stack, Productivity,
    SaaS, Technology, Enterprise, API Provider, Profiles, Publish, Service API, Relative
    Data, Relative StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/collections-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/collections-get-openapi.md
- name: Box - Get Collection Items
  x-api-slug: collectionscollection-iditems-get
  description: |-
    Retrieves the files and/or folders contained within this collection. Collection item lists behave a lot like getting a folder???s items.
    Paginated results can be retrieved using the limit and offset parameters.
    Sub-object fields can be requested via the ?fields parameter
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files, Collaboration, Sharing, Storage, Storage, Stack Network, Stack, Productivity,
    SaaS, Technology, Enterprise, API Provider, Profiles, Publish, Service API, Relative
    Data, Relative StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/collectionscollection-iditems-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/collectionscollection-iditems-get-openapi.md
- name: Box - Get Comment
  x-api-slug: commentscomment-id-get
  description: Used to retrieve the message and metadata about a specific comment.
    Information about the user who created the comment is also included.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files, Collaboration, Sharing, Storage, Storage, Stack Network, Stack, Productivity,
    SaaS, Technology, Enterprise, API Provider, Profiles, Publish, Service API, Relative
    Data, Relative StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/commentscomment-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/commentscomment-id-get-openapi.md
- name: Box - Delete Comment
  x-api-slug: commentscomment-id-delete
  description: Permanently deletes a comment.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files, Collaboration, Sharing, Storage, Storage, Stack Network, Stack, Productivity,
    SaaS, Technology, Enterprise, API Provider, Profiles, Publish, Service API, Relative
    Data, Relative StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/commentscomment-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/commentscomment-id-delete-openapi.md
- name: Box - Get Task
  x-api-slug: taskstask-id-get
  description: Fetches a specific task.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files, Collaboration, Sharing, Storage, Storage, Stack Network, Stack, Productivity,
    SaaS, Technology, Enterprise, API Provider, Profiles, Publish, Service API, Relative
    Data, Relative StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/taskstask-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/taskstask-id-get-openapi.md
- name: Box - Delete Task
  x-api-slug: taskstask-id-delete
  description: Permanently deletes a specific task.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files, Collaboration, Sharing, Storage, Storage, Stack Network, Stack, Productivity,
    SaaS, Technology, Enterprise, API Provider, Profiles, Publish, Service API, Relative
    Data, Relative StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/taskstask-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/taskstask-id-delete-openapi.md
- name: Box - Get Assignments
  x-api-slug: taskstask-idassignments-get
  description: Retrieves all of the assignments for a given task.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files, Collaboration, Sharing, Storage, Storage, Stack Network, Stack, Productivity,
    SaaS, Technology, Enterprise, API Provider, Profiles, Publish, Service API, Relative
    Data, Relative StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/taskstask-idassignments-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/taskstask-idassignments-get-openapi.md
- name: Box - Get Task Assignment
  x-api-slug: task-assignmentstask-assignment-id-get
  description: Fetches a specific task assignment.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files, Collaboration, Sharing, Storage, Storage, Stack Network, Stack, Productivity,
    SaaS, Technology, Enterprise, API Provider, Profiles, Publish, Service API, Relative
    Data, Relative StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/task-assignmentstask-assignment-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/task-assignmentstask-assignment-id-get-openapi.md
- name: Box - Delete Task Assignment
  x-api-slug: task-assignmentstask-assignment-id-delete
  description: Deletes a specific task assignment.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files, Collaboration, Sharing, Storage, Storage, Stack Network, Stack, Productivity,
    SaaS, Technology, Enterprise, API Provider, Profiles, Publish, Service API, Relative
    Data, Relative StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/task-assignmentstask-assignment-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/task-assignmentstask-assignment-id-delete-openapi.md
- name: Box - User Events, Enterprise Events
  x-api-slug: events-get
  description: |-
    Use this to get events for a given user. A chunk of event objects is returned for the user based on the parameters passed in. Parameters indicating how many chunks are left as well as the next stream_position are also returned.

    To retrieve Enterprise Events specify 'stream_type=admin_logs'. Retrieves up to a year' events for all users in an enterprise. Upper and lower bounds as well as filters can be applied to the results.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files, Collaboration, Sharing, Storage, Storage, Stack Network, Stack, Productivity,
    SaaS, Technology, Enterprise, API Provider, Profiles, Publish, Service API, Relative
    Data, Relative StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/events-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/events-get-openapi.md
- name: Box - Long polling
  x-api-slug: events-options
  description: |-
    To get real-time notification of activity in a Box account, use the long poll feature of the /events API. To do so, first call the /events API with an OPTIONS call to retrieve the long poll URL to use. Next, make a GET request to the provided URL to begin listening for events. If an event occurs within an account you are monitoring, you will receive a response with the value new_change. It???s important to note that this response will not come with any other details, but should serve as a prompt to take further action such as calling the /events endpoint with your last known stream_position. After sending this response, the server will close the connection and you will need to repeat the long poll process to begin listening for events again.
    If no events occur for a period of time after you make the GET request to the long poll URL, you will receive a response with the value reconnect. When you receive this response, you???ll make another OPTIONS call to the /events endpoint and repeat the long poll process.
    If you receive no events in retry_timeout seconds, you should make another GET request to the real time server (i.e. URL in the response). This might be necessary in case you do not receive the reconnect message in the face of network errors.
    If you receive max_retries error when making GET requests to the real time server, you should make another OPTIONS request.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files, Collaboration, Sharing, Storage, Storage, Stack Network, Stack, Productivity,
    SaaS, Technology, Enterprise, API Provider, Profiles, Publish, Service API, Relative
    Data, Relative StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/events-options-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/events-options-openapi.md
- name: Box - Get Enterprise Users
  x-api-slug: users-get
  description: Returns a list of all users for the Enterprise along with their user_id,
    public_name, and login.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files, Collaboration, Sharing, Storage, Storage, Stack Network, Stack, Productivity,
    SaaS, Technology, Enterprise, API Provider, Profiles, Publish, Service API, Relative
    Data, Relative StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/users-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/users-get-openapi.md
- name: Box - Get Current User
  x-api-slug: usersme-get
  description: Retrieves information about the user who is currently logged in i.e.
    the user for whom this auth token was generated.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files, Collaboration, Sharing, Storage, Storage, Stack Network, Stack, Productivity,
    SaaS, Technology, Enterprise, API Provider, Profiles, Publish, Service API, Relative
    Data, Relative StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/usersme-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/usersme-get-openapi.md
- name: Box - Get User's Info
  x-api-slug: usersuser-id-get
  description: Retrieves information about a user in the enterprise. Requires enterprise
    administration authorization.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files, Collaboration, Sharing, Storage, Storage, Stack Network, Stack, Productivity,
    SaaS, Technology, Enterprise, API Provider, Profiles, Publish, Service API, Relative
    Data, Relative StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/usersuser-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/usersuser-id-get-openapi.md
- name: Box - Delete User
  x-api-slug: usersuser-id-delete
  description: Deletes a user in an enterprise account.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files, Collaboration, Sharing, Storage, Storage, Stack Network, Stack, Productivity,
    SaaS, Technology, Enterprise, API Provider, Profiles, Publish, Service API, Relative
    Data, Relative StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/usersuser-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/usersuser-id-delete-openapi.md
- name: Box - Get Email Aliases
  x-api-slug: usersuser-idemail-aliases-get
  description: Retrieves all email aliases for this user. The collection of email
    aliases does not include the primary login for the user; use GET /users/USER_ID
    to retrieve the login email address.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files, Collaboration, Sharing, Storage, Storage, Stack Network, Stack, Productivity,
    SaaS, Technology, Enterprise, API Provider, Profiles, Publish, Service API, Relative
    Data, Relative StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/usersuser-idemail-aliases-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/usersuser-idemail-aliases-get-openapi.md
- name: Box - Delete Email Alias
  x-api-slug: usersuser-idemail-aliasesemail-alias-id-delete
  description: Removes an email alias from a user.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files, Collaboration, Sharing, Storage, Storage, Stack Network, Stack, Productivity,
    SaaS, Technology, Enterprise, API Provider, Profiles, Publish, Service API, Relative
    Data, Relative StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/usersuser-idemail-aliasesemail-alias-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/usersuser-idemail-aliasesemail-alias-id-delete-openapi.md
- name: Box - Get status of the invite
  x-api-slug: invitesinvite-id-get
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files, Collaboration, Sharing, Storage, Storage, Stack Network, Stack, Productivity,
    SaaS, Technology, Enterprise, API Provider, Profiles, Publish, Service API, Relative
    Data, Relative StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/invitesinvite-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/invitesinvite-id-get-openapi.md
- name: Box - Get Groups for an Enterprise
  x-api-slug: groups-get
  description: Retrieves all of the groups for given enterprise. Must have permissions
    to see an enterprise's groups.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files, Collaboration, Sharing, Storage, Storage, Stack Network, Stack, Productivity,
    SaaS, Technology, Enterprise, API Provider, Profiles, Publish, Service API, Relative
    Data, Relative StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/groups-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/groups-get-openapi.md
- name: Box - Get Group
  x-api-slug: groupsgroup-id-get
  description: Used to get information about a group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files, Collaboration, Sharing, Storage, Storage, Stack Network, Stack, Productivity,
    SaaS, Technology, Enterprise, API Provider, Profiles, Publish, Service API, Relative
    Data, Relative StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/groupsgroup-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/groupsgroup-id-get-openapi.md
- name: Box - Delete Group
  x-api-slug: groupsgroup-id-delete
  description: Permanently deletes a specific group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files, Collaboration, Sharing, Storage, Storage, Stack Network, Stack, Productivity,
    SaaS, Technology, Enterprise, API Provider, Profiles, Publish, Service API, Relative
    Data, Relative StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/groupsgroup-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/groupsgroup-id-delete-openapi.md
- name: Box - Get Membership
  x-api-slug: group-membershipsgroup-membership-id-get
  description: Fetches a specific group membership entry.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files, Collaboration, Sharing, Storage, Storage, Stack Network, Stack, Productivity,
    SaaS, Technology, Enterprise, API Provider, Profiles, Publish, Service API, Relative
    Data, Relative StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/group-membershipsgroup-membership-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/group-membershipsgroup-membership-id-get-openapi.md
- name: Box - Delete Membership
  x-api-slug: group-membershipsgroup-membership-id-delete
  description: Deletes a specific group membership.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files, Collaboration, Sharing, Storage, Storage, Stack Network, Stack, Productivity,
    SaaS, Technology, Enterprise, API Provider, Profiles, Publish, Service API, Relative
    Data, Relative StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/group-membershipsgroup-membership-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/group-membershipsgroup-membership-id-delete-openapi.md
- name: Box - Get Memberships for Group
  x-api-slug: groupsgroup-idmemberships-get
  description: Retrieves all of the members for a given group if the requesting user
    has access (see Group Object member_viewability_level).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files, Collaboration, Sharing, Storage, Storage, Stack Network, Stack, Productivity,
    SaaS, Technology, Enterprise, API Provider, Profiles, Publish, Service API, Relative
    Data, Relative StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/groupsgroup-idmemberships-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/groupsgroup-idmemberships-get-openapi.md
- name: Box - Get Memberships for User
  x-api-slug: usersuser-idmemberships-get
  description: Retrieves all of the group memberships for a given user. Note this
    is only available to group admins. To retrieve group memberships for the user
    making the API request, use the users/me/memberships endpoint.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files, Collaboration, Sharing, Storage, Storage, Stack Network, Stack, Productivity,
    SaaS, Technology, Enterprise, API Provider, Profiles, Publish, Service API, Relative
    Data, Relative StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/usersuser-idmemberships-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/usersuser-idmemberships-get-openapi.md
- name: Box - Get Collaborations for Group
  x-api-slug: groupsgroup-idcollaborations-get
  description: Retrieves all of the group collaborations for a given group. Note this
    is only available to group admins.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files, Collaboration, Sharing, Storage, Storage, Stack Network, Stack, Productivity,
    SaaS, Technology, Enterprise, API Provider, Profiles, Publish, Service API, Relative
    Data, Relative StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/groupsgroup-idcollaborations-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/groupsgroup-idcollaborations-get-openapi.md
- name: Box - Get Enterprise Device Pins
  x-api-slug: enterprisesenterprise-iddevice-pinners-get
  description: Gets all the device pins within a given enterprise. Must be an enterprise
    admin with the manage enterprise scope to make this call.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files, Collaboration, Sharing, Storage, Storage, Stack Network, Stack, Productivity,
    SaaS, Technology, Enterprise, API Provider, Profiles, Publish, Service API, Relative
    Data, Relative StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/enterprisesenterprise-iddevice-pinners-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/enterprisesenterprise-iddevice-pinners-get-openapi.md
- name: Box - Get Device Pin
  x-api-slug: device-pinnersid-get
  description: Gets information about an individual device pin.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files, Collaboration, Sharing, Storage, Storage, Stack Network, Stack, Productivity,
    SaaS, Technology, Enterprise, API Provider, Profiles, Publish, Service API, Relative
    Data, Relative StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/device-pinnersid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/device-pinnersid-get-openapi.md
- name: Box - Delete Device Pin
  x-api-slug: device-pinnersid-delete
  description: Delete individual device pin.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files, Collaboration, Sharing, Storage, Storage, Stack Network, Stack, Productivity,
    SaaS, Technology, Enterprise, API Provider, Profiles, Publish, Service API, Relative
    Data, Relative StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/device-pinnersid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/device-pinnersid-delete-openapi.md
- name: Box - Get Retention Policies
  x-api-slug: retention-policies-get
  description: Retrieves all of the retention policies for the given enterprise.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files, Collaboration, Sharing, Storage, Storage, Stack Network, Stack, Productivity,
    SaaS, Technology, Enterprise, API Provider, Profiles, Publish, Service API, Relative
    Data, Relative StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/retention-policies-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/retention-policies-get-openapi.md
- name: Box - Get Retention Policy
  x-api-slug: retention-policiespolicy-id-get
  description: Used to retrieve information about a retention policy
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files, Collaboration, Sharing, Storage, Storage, Stack Network, Stack, Productivity,
    SaaS, Technology, Enterprise, API Provider, Profiles, Publish, Service API, Relative
    Data, Relative StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/retention-policiespolicy-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/retention-policiespolicy-id-get-openapi.md
- name: Box - Get Retention Policy Assignments
  x-api-slug: retention-policiespolicy-idassignments-get
  description: Returns a list of all retention policy assignments associated with
    a specified retention policy.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files, Collaboration, Sharing, Storage, Storage, Stack Network, Stack, Productivity,
    SaaS, Technology, Enterprise, API Provider, Profiles, Publish, Service API, Relative
    Data, Relative StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/retention-policiespolicy-idassignments-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/retention-policiespolicy-idassignments-get-openapi.md
- name: Box - Get Retention Policy Assignment
  x-api-slug: retention-policy-assignmentsretention-policy-assignment-id-get
  description: Used to retrieve information about a retention policy assignment.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files, Collaboration, Sharing, Storage, Storage, Stack Network, Stack, Productivity,
    SaaS, Technology, Enterprise, API Provider, Profiles, Publish, Service API, Relative
    Data, Relative StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/retention-policy-assignmentsretention-policy-assignment-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/retention-policy-assignmentsretention-policy-assignment-id-get-openapi.md
- name: Box - Get File Version Retentions
  x-api-slug: file-version-retentions-get
  description: Retrieves all file version retentions for the given enterprise.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files, Collaboration, Sharing, Storage, Storage, Stack Network, Stack, Productivity,
    SaaS, Technology, Enterprise, API Provider, Profiles, Publish, Service API, Relative
    Data, Relative StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/file-version-retentions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/file-version-retentions-get-openapi.md
- name: Box - Get File Version Retention
  x-api-slug: file-version-retentionsfile-version-retention-id-get
  description: Used to retrieve information about a file version retention
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files, Collaboration, Sharing, Storage, Storage, Stack Network, Stack, Productivity,
    SaaS, Technology, Enterprise, API Provider, Profiles, Publish, Service API, Relative
    Data, Relative StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/file-version-retentionsfile-version-retention-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/file-version-retentionsfile-version-retention-id-get-openapi.md
- name: Box - Get Legal Hold Policies
  x-api-slug: legal-hold-policies-get
  description: Get a list of Legal Hold Policies that belong to your Enterprise.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files, Collaboration, Sharing, Storage, Storage, Stack Network, Stack, Productivity,
    SaaS, Technology, Enterprise, API Provider, Profiles, Publish, Service API, Relative
    Data, Relative StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/legal-hold-policies-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/legal-hold-policies-get-openapi.md
- name: Box - Get Legal Hold Policy
  x-api-slug: legal-hold-policiesid-get
  description: Get details of a single Legal Hold Policy
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files, Collaboration, Sharing, Storage, Storage, Stack Network, Stack, Productivity,
    SaaS, Technology, Enterprise, API Provider, Profiles, Publish, Service API, Relative
    Data, Relative StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/legal-hold-policiesid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/legal-hold-policiesid-get-openapi.md
- name: Box - Delete Legal Hold Policy
  x-api-slug: legal-hold-policiesid-delete
  description: Sends request to delete an existing Legal Hold Policy. Note that this
    is an asynchronous process - the Policy will not be fully deleted yet when the
    response comes back.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files, Collaboration, Sharing, Storage, Storage, Stack Network, Stack, Productivity,
    SaaS, Technology, Enterprise, API Provider, Profiles, Publish, Service API, Relative
    Data, Relative StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/legal-hold-policiesid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/legal-hold-policiesid-delete-openapi.md
- name: Box - Get Legal hold policy assignments
  x-api-slug: legal-hold-policiesidassignments-get
  description: Get list of assignments for a single Policy.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files, Collaboration, Sharing, Storage, Storage, Stack Network, Stack, Productivity,
    SaaS, Technology, Enterprise, API Provider, Profiles, Publish, Service API, Relative
    Data, Relative StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/legal-hold-policiesidassignments-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/legal-hold-policiesidassignments-get-openapi.md
- name: Box - Get Legal Hold Policy Assignment
  x-api-slug: legal-hold-policy-assignmentsassignment-id-get
  description: Get details of a single assignment.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files, Collaboration, Sharing, Storage, Storage, Stack Network, Stack, Productivity,
    SaaS, Technology, Enterprise, API Provider, Profiles, Publish, Service API, Relative
    Data, Relative StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/legal-hold-policy-assignmentsassignment-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/legal-hold-policy-assignmentsassignment-id-get-openapi.md
- name: Box - Delete Legal Hold Policy Assignment
  x-api-slug: legal-hold-policy-assignmentsassignment-id-delete
  description: Sends request to delete an existing Assignment. Note that this is an
    asynchronous process - the Assignment will not be fully deleted yet when the response
    comes back.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files, Collaboration, Sharing, Storage, Storage, Stack Network, Stack, Productivity,
    SaaS, Technology, Enterprise, API Provider, Profiles, Publish, Service API, Relative
    Data, Relative StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/legal-hold-policy-assignmentsassignment-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/legal-hold-policy-assignmentsassignment-id-delete-openapi.md
- name: Box - Get List of File Version Legal Holds
  x-api-slug: file-version-legal-holds-get
  description: Get list of non-deleted Holds for a single Policy.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files, Collaboration, Sharing, Storage, Storage, Stack Network, Stack, Productivity,
    SaaS, Technology, Enterprise, API Provider, Profiles, Publish, Service API, Relative
    Data, Relative StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/file-version-legal-holds-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/file-version-legal-holds-get-openapi.md
- name: Box - Get File Version Legal Hold
  x-api-slug: file-version-legal-holdsid-get
  description: Get details of a single File Version Legal Hold.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files, Collaboration, Sharing, Storage, Storage, Stack Network, Stack, Productivity,
    SaaS, Technology, Enterprise, API Provider, Profiles, Publish, Service API, Relative
    Data, Relative StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/file-version-legal-holdsid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/file-version-legal-holdsid-get-openapi.md
- name: Box - Get Webhooks
  x-api-slug: webhooks-get
  description: |-
    Returns all defined webhooks for the requesting application and user, up to the limit. If no limit is supplied then Box uses the default limit of 100.
    If more than limit webhooks are defined then Box returns the webhooks in batches. When the results are batched, Box sends limit webhooks along with a next_marker field in the response object. The value of the next_marker field is a marker string that you can use in later requests to tell Box which batch to send next.
    When you send a request that includes a marker string, Box sends the next batch of webhooks, beginning after the last webhook of the previous batch. When the response contains the last of the defined webhooks, Box omits the next_marker field from its response.
    You can use limit and marker together with the marker string returned in the next_marker field to paginate lists of webhooks.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files, Collaboration, Sharing, Storage, Storage, Stack Network, Stack, Productivity,
    SaaS, Technology, Enterprise, API Provider, Profiles, Publish, Service API, Relative
    Data, Relative StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/webhooks-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/webhooks-get-openapi.md
- name: Box - Get Webhook
  x-api-slug: webhookswebhook-id-get
  description: Get a Webhook
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files, Collaboration, Sharing, Storage, Storage, Stack Network, Stack, Productivity,
    SaaS, Technology, Enterprise, API Provider, Profiles, Publish, Service API, Relative
    Data, Relative StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/webhookswebhook-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/webhookswebhook-id-get-openapi.md
- name: Box - Delete Webhook
  x-api-slug: webhookswebhook-id-delete
  description: Permanently deletes a webhook
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Files, Collaboration, Sharing, Storage, Storage, Stack Network, Stack, Productivity,
    SaaS, Technology, Enterprise, API Provider, Profiles, Publish, Service API, Relative
    Data, Relative StreamRank, Streams, Backups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/webhookswebhook-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/webhookswebhook-id-delete-openapi.md
x-common:
- type: x-api-gallery
  url: http://botify.api.gallery.streamdata.io
- type: x-api-stack
  url: http://box.stack.network
- type: x-base
  url: https://api.box.com/
- type: x-blog
  url: http://blog.box.com/
- type: x-blog-rss
  url: http://blog.box.com/feed/
- type: x-crunchbase
  url: http://www.crunchbase.com/company/box
- type: x-crunchbase
  url: https://crunchbase.com/organization/box
- type: x-developer
  url: http://developers.box.com
- type: x-github
  url: https://github.com/box
- type: x-pricing
  url: https://developers.box.com/box-platform-pricing/
- type: x-road-map
  url: https://developers.box.com/roadmap/
- type: x-twitter
  url: https://twitter.com/BoxPlatform
- type: x-twitter
  url: https://twitter.com/BoxHQ
- type: x-website
  url: http://box.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---