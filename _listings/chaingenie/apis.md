---
name: ChainGenie
x-slug: chaingenie
description: ChainGenie provides a plug and play platform that helps you connect your
  existing (or create new) applications to DLTs for lodging and workflow management
  using a simple easy to use user interface. ChainGenie is a platform to create blockchain
  apps that provide speed-to-market for companies looking to launch faster, rather
  than reinvent the wheel. Write your applications to run on popular Blockchain networks
  like Ethereum, Bitcoin Blockchain etc with great ease when you require to validate
  credentials or make your existing traditional applications use the power of DLT
  and blockchain overnight!
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28902-api-chaingenie-com.jpg
x-kinRank: "7"
x-alexaRank: ""
tags: Documents
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/chaingenie/apis.md
specificationVersion: "0.14"
apis:
- name: ChainGenie = DLT + Blockchain + Magic - Retrieve document from IPFS
  x-api-slug: ethledgeripfsget-post
  description: Retrieve the document stream from IPFS node
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28902-api-chaingenie-com.jpg
  humanURL: http://chaingenie.com
  baseURL: https://api.chaingenie.com//api/v1
  tags: Blockchain
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/chaingenie/ethledgeripfsget-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/chaingenie/ethledgeripfsget-post-openapi.md
- name: ChainGenie = DLT + Blockchain + Magic - Write document to IPFS
  x-api-slug: ethledgeripfsadd-post
  description: Post the document into ipfs for safekeep!
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28902-api-chaingenie-com.jpg
  humanURL: http://chaingenie.com
  baseURL: https://api.chaingenie.com//api/v1
  tags: Blockchain
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/chaingenie/ethledgeripfsadd-post-openapi.md
- name: ChainGenie = DLT + Blockchain + Magic - Document transactions
  x-api-slug: ethledgergettrans-get
  description: Displays all transactions connected to this project / smart contract
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28902-api-chaingenie-com.jpg
  humanURL: http://chaingenie.com
  baseURL: https://api.chaingenie.com//api/v1
  tags: Blockchain
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/chaingenie/ethledgergettrans-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/chaingenie/ethledgergettrans-get-openapi.md
- name: ChainGenie = DLT + Blockchain + Magic - Get document status using hash
  x-api-slug: ethledgergetdocstate-post
  description: Review the document status - existence, hash, block info, signatories,
    routing to users and details
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28902-api-chaingenie-com.jpg
  humanURL: http://chaingenie.com
  baseURL: https://api.chaingenie.com//api/v1
  tags: Blockchain
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/chaingenie/ethledgergetdocstate-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/chaingenie/ethledgergetdocstate-post-openapi.md
- name: ChainGenie = DLT + Blockchain + Magic - Sign document using hash (min fn;
    no return)
  x-api-slug: ethledgersigncert-post
  description: Cryptographically sign the document and add the record to blockchain.  The
    document history and status is updated for querying.  The API call does not return
    any document properties.  This is a <b>minimalistic function</b> for stringing
    with other functions
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28902-api-chaingenie-com.jpg
  humanURL: http://chaingenie.com
  baseURL: https://api.chaingenie.com//api/v1
  tags: Blockchain
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/chaingenie/ethledgersigncert-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/chaingenie/ethledgersigncert-post-openapi.md
- name: ChainGenie = DLT + Blockchain + Magic - Send document using hash (min fn;
    no return)
  x-api-slug: ethledgersendcert-post
  description: Route the document to a recipient.  The document history and status
    is updated for querying.  The API call does not return any document properties.  This
    is a <b>minimalistic function</b> for stringing with other functions
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28902-api-chaingenie-com.jpg
  humanURL: http://chaingenie.com
  baseURL: https://api.chaingenie.com//api/v1
  tags: Blockchain
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/chaingenie/ethledgersendcert-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/chaingenie/ethledgersendcert-post-openapi.md
- name: ChainGenie = DLT + Blockchain + Magic - Post document to IPFS + blockchain
  x-api-slug: ethledgerpostdoc-post
  description: Post document hash into eth chain for POE (proof of existence) and
    post the document into ipfs for safekeep!
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28902-api-chaingenie-com.jpg
  humanURL: http://chaingenie.com
  baseURL: https://api.chaingenie.com//api/v1
  tags: Blockchain
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/chaingenie/ethledgerpostdoc-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/chaingenie/ethledgerpostdoc-post-openapi.md
- name: ChainGenie = DLT + Blockchain + Magic - Check document exists on blockchain
  x-api-slug: ethledgerexistsdoc-post
  description: Check if your documents exists in the eth blockchain
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28902-api-chaingenie-com.jpg
  humanURL: http://chaingenie.com
  baseURL: https://api.chaingenie.com//api/v1
  tags: Blockchain
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/chaingenie/ethledgerexistsdoc-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/chaingenie/ethledgerexistsdoc-post-openapi.md
- name: ChainGenie = DLT + Blockchain + Magic - Get document status with file
  x-api-slug: ethledgerdocstatus-post
  description: Review the document status - existence, hash, block info, signatories,
    routing to users and details
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28902-api-chaingenie-com.jpg
  humanURL: http://chaingenie.com
  baseURL: https://api.chaingenie.com//api/v1
  tags: Blockchain
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/chaingenie/ethledgerdocstatus-post-openapi.md
- name: ChainGenie = DLT + Blockchain + Magic - Sign document
  x-api-slug: ethledgersign-post
  description: Cryptographically sign the document and add the record to blockchain.  The
    document history and status is updated for querying.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28902-api-chaingenie-com.jpg
  humanURL: http://chaingenie.com
  baseURL: https://api.chaingenie.com//api/v1
  tags: Blockchain
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/chaingenie/ethledgersign-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/chaingenie/ethledgersign-post-openapi.md
- name: ChainGenie = DLT + Blockchain + Magic - Send document
  x-api-slug: ethledgersendforsign-post
  description: Route the document for signature.  The document history and status
    is updated for querying.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28902-api-chaingenie-com.jpg
  humanURL: http://chaingenie.com
  baseURL: https://api.chaingenie.com//api/v1
  tags: Blockchain
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/chaingenie/ethledgersendforsign-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/chaingenie/ethledgersendforsign-post-openapi.md
- name: ChainGenie = DLT + Blockchain + Magic - Generate and Manage Document (Basic)
  x-api-slug: ethledgerdocert-post
  description: "This is an over simplified version for testing this API for its powers
    a template - uses an inbuilt into ChainGenie template and values are preconfigured
    - just running this will work and provide you an IPFS handle to retrieve the document
    you generated with your variables / values from the template.\nUse an existing
    document on our server and generate a document with automated sign and routing
    to a recipient.  Ex. this configured api will generate a certificate for a student
    name (name) with the completed certificate course (course) and dated (date). \nThe
    document hash will be posted on blockchain and the actual document will be added
    to IPFS.  Want to retrieve your document? Check out the API - Write & Retrieve
    - Docs (IPFS)."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28902-api-chaingenie-com.jpg
  humanURL: http://chaingenie.com
  baseURL: https://api.chaingenie.com//api/v1
  tags: Blockchain
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/chaingenie/ethledgerdocert-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/chaingenie/ethledgerdocert-post-openapi.md
- name: ChainGenie = DLT + Blockchain + Magic - Generate, Sign & Route Document (Advanced)
  x-api-slug: ethledgerinvokecontract-post
  description: "This API is the generic version of the \"Generate document from template\"
    API. Any template file can be uploaded (sample available as link for testing).
    \ If you just want to see how this would work - use the other call and just run
    it without any uploaded certificate. \nUpload a templated pdf with editable /
    filable fields and generate a document with automated sign and routing to a recipient.
    \ Every attribute that needs to be filled will need to be passed in the format
    - ex. course field to be substituted - field = attrib; value = [\"course\",\"course
    value\"] or date field to be substituted - field = attrib; value = [\"date\",\"12/12/2016\"].
    \ If your fillable form has the field named \"today\", current time will be used
    for filling the value of that field.\nYou will need to upload for the file attribute
    a real template file with fillable fields. For the sample values as configured,
    you can use the demo template available at http://chaingenie.com/cert.pdf.  Download
    this certificate and add it as your input file\nTo route the document to recipient
    (optional) add field recipient with \"key\" of the recipient - available recipient
    in the system - 0xb3A214341df9560a3e09E256BfacefD6648f5Ca9 for your testing\nUse
    case - Upload an invoice template with fillable fields, add attrib values for
    all the fields that needs to be filled, add the recipient field - your invoice
    will be created, signed with your key (in production / in test it will be signed
    with the local admin key) and will be routed to the recipient (in production you
    can add your recipient / in sandbox - use recipient 0xb3A214341df9560a3e09E256BfacefD6648f5Ca9)\nResponse
    will contain the document name, signatories, timestamps, recipient, IPFS hash
    (handle to retrieve the actual document)\nThe document hash will be posted on
    blockchain and the actual document will be added to IPFS.  Want to retrieve your
    document? Check out the API - Write & Retrieve - Docs (IPFS)."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28902-api-chaingenie-com.jpg
  humanURL: http://chaingenie.com
  baseURL: https://api.chaingenie.com//api/v1
  tags: Blockchain
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/chaingenie/ethledgerinvokecontract-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/chaingenie/ethledgerinvokecontract-post-openapi.md
x-common:
- type: x-github
  url: https://github.com/ChainGenie
- type: x-website
  url: http://chaingenie.com
- type: x-api-gallery
  url: http://broadleaf.commerce.api.gallery.streamdata.io
- type: x-twitter
  url: https://twitter.com/ChainGenie
- type: x-website
  url: http://api.chaingenie.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---