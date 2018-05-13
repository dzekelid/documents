---
name: Box
description: Box Inc. (formerly Box.net) is an online file sharing and Cloud content
  management service for enterprise companies. The company has adopted a freemium
  business model, and provides 5 GB of free storage [3] for personal accounts. A mobile
  version of the service is available for Android, BlackBerry, iOS, WebOS, and Windows
  Phone devices. The company is based in Los Altos, California.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/box1200x630.jpg
x-kinRank: "9"
x-alexaRank: ""
tags:
- Storage
- Storage
- Stack Network
- Stack
- Sharing
- Road Map
- Publishing
- Productivity
- Files
- Collaboration
- Backup
created: "2018-03-23"
modified: "2018-03-23"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/apis.yaml
specificationVersion: "0.14"
apis:
- name: Box
  description: Box Inc
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/box1200x630.jpg
  humanURL: ""
  baseURL: https://api.box.com//2.0
  tags: Documents
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/webhooks-webhook-id-delete.md
- name: Box Update Folder, Create Shared Link, Create or Delete
  description: "Used to update information about the folder. To move a folder, update
    the ID of its parent. To enable an email address that can be used to upload files
    to this folder, update the folder_upload_email attribute. An optional If-Match
    header can be included to ensure that client only updates the folder if it knows
    about the latest version.\n\nUsed to create a shared link for this particular
    folder. Please see here for more information on the permissions available for
    shared links. In order to get default shared link status, set it to an empty access
    level, i.e. {\"shared_link\": {}}. In order to disable a shared link, send this
    same type of PUT request with the value of shared_link set to null, i.e. {\"shared_link\":
    null}\n\nTo add or remove an item from a collection, you do a PUT on that item
    and change the list of collections it belongs to. Philosophically, this is similar
    to the way \u201Cmove\u201D operations work on files and folders: you do a PUT
    on the item and change its parent. It\u2019s the same idea with collections, except
    you\u2019re changing which collection(s) the item belongs to instead of the folder
    it belongs to. Currently the only collection available is the favorites collection,
    and you\u2019ll need to know it\u2019s ID for the user that is making the API
    call, since every user has a different favorites collection_id.\nThe Add/Remove
    API handling will check all ids passed in before performing any add/removal operations.
    If any collection ids are malformed or do not exist in the user\u2019s account,
    the API call will throw a 400. Only if all of the collection ids are valid will
    the adds and removals be carried out."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/box1200x630.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Documents
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/folders-folder-id-put.md
x-common:
- type: x-base
  url: https://api.box.com/
- type: x-blog
  url: http://blog.box.com/
- type: x-blog-rss
  url: http://blog.box.com/feed/
- type: x-crunchbase
  url: http://www.crunchbase.com/company/box
- type: x-developer
  url: http://developers.box.com
- type: x-github
  url: https://github.com/boxdotnet
- type: x-pricing
  url: https://developers.box.com/box-platform-pricing/
- type: x-road-map
  url: https://developers.box.com/roadmap/
- type: x-twitter
  url: https://twitter.com/BoxPlatform
- type: x-website
  url: http://box.com
- type: x-base
  url: https://api.box.com/
- type: x-blog
  url: http://blog.box.com/
- type: x-blog-rss
  url: http://blog.box.com/feed/
- type: x-crunchbase
  url: http://www.crunchbase.com/company/box
- type: x-developer
  url: http://developers.box.com
- type: x-github
  url: https://github.com/boxdotnet
- type: x-pricing
  url: https://developers.box.com/box-platform-pricing/
- type: x-road-map
  url: https://developers.box.com/roadmap/
- type: x-twitter
  url: https://twitter.com/BoxPlatform
- type: x-website
  url: http://box.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---