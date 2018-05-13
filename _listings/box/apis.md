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
- name: Box Delete Web Link
  description: Deletes a web link and moves it to the trash
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/box1200x630.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Documents
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/web-links-web-link-id-delete.md
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/web-links-web-link-id-delete-postman.md
- name: Box Long polling
  description: "To get real-time notification of activity in a Box account, use the
    long poll feature of the /events API. To do so, first call the /events API with
    an OPTIONS call to retrieve the long poll URL to use. Next, make a GET request
    to the provided URL to begin listening for events. If an event occurs within an
    account you are monitoring, you will receive a response with the value new_change.
    It\u2019s important to note that this response will not come with any other details,
    but should serve as a prompt to take further action such as calling the /events
    endpoint with your last known stream_position. After sending this response, the
    server will close the connection and you will need to repeat the long poll process
    to begin listening for events again.\nIf no events occur for a period of time
    after you make the GET request to the long poll URL, you will receive a response
    with the value reconnect. When you receive this response, you\u2019ll make another
    OPTIONS call to the /events endpoint and repeat the long poll process.\nIf you
    receive no events in retry_timeout seconds, you should make another GET request
    to the real time server (i.e. URL in the response). This might be necessary in
    case you do not receive the reconnect message in the face of network errors.\nIf
    you receive max_retries error when making GET requests to the real time server,
    you should make another OPTIONS request."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/box1200x630.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Documents
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/events-options.md
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/box/events-options-postman.md
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