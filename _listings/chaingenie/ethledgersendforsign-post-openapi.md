---
swagger: "2.0"
x-collection-name: ChainGenie
x-complete: 0
info:
  title: ChainGenie Send document
  description: Route the document for signature.  The document history and status
    is updated for querying.
  version: "1.0"
host: api.chaingenie.com
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /ethledger/ipfsget:
    post:
      summary: Retrieve document from IPFS
      description: Retrieve the document stream from IPFS node
      operationId: EthledgerIpfsgetPost
      x-api-path-slug: ethledgeripfsget-post
      parameters:
      - in: header
        name: ApiKey
      - in: formData
        name: hash
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Retrieve
      - Document
      - From
      - IPFS
  /ethledger/ipfsadd:
    post:
      summary: Write document to IPFS
      description: Post the document into ipfs for safekeep!
      operationId: EthledgerIpfsaddPost
      x-api-path-slug: ethledgeripfsadd-post
      parameters:
      - in: header
        name: ApiKey
      - in: formData
        name: files
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Write
      - Document
      - To
      - IPFS
  /ethledger/gettrans:
    get:
      summary: Document transactions
      description: Displays all transactions connected to this project / smart contract
      operationId: EthledgerGettransGet
      x-api-path-slug: ethledgergettrans-get
      parameters:
      - in: header
        name: ApiKey
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Document
      - Transactions
  /ethledger/getdocstate:
    post:
      summary: Get document status using hash
      description: Review the document status - existence, hash, block info, signatories,
        routing to users and details
      operationId: EthledgerGetdocstatePost
      x-api-path-slug: ethledgergetdocstate-post
      parameters:
      - in: header
        name: ApiKey
      - in: formData
        name: strHash
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Document
      - Status
      - Using
      - Hash
  /ethledger/signcert:
    post:
      summary: Sign document using hash (min fn; no return)
      description: Cryptographically sign the document and add the record to blockchain.  The
        document history and status is updated for querying.  The API call does not
        return any document properties.  This is a <b>minimalistic function</b> for
        stringing with other functions
      operationId: EthledgerSigncertPost
      x-api-path-slug: ethledgersigncert-post
      parameters:
      - in: header
        name: ApiKey
      - in: formData
        name: strHash
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Sign
      - Document
      - Using
      - Hash
      - (min
      - Fn;
      - "No"
      - Return)
  /ethledger/sendcert:
    post:
      summary: Send document using hash (min fn; no return)
      description: Route the document to a recipient.  The document history and status
        is updated for querying.  The API call does not return any document properties.  This
        is a <b>minimalistic function</b> for stringing with other functions
      operationId: EthledgerSendcertPost
      x-api-path-slug: ethledgersendcert-post
      parameters:
      - in: header
        name: ApiKey
      - in: formData
        name: recipient
      - in: formData
        name: strHash
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Send
      - Document
      - Using
      - Hash
      - (min
      - Fn;
      - "No"
      - Return)
  /ethledger/postdoc:
    post:
      summary: Post document to IPFS + blockchain
      description: Post document hash into eth chain for POE (proof of existence)
        and post the document into ipfs for safekeep!
      operationId: EthledgerPostdocPost
      x-api-path-slug: ethledgerpostdoc-post
      parameters:
      - in: header
        name: ApiKey
      - in: formData
        name: files
      - in: formData
        name: filetypes
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Document
      - To
      - IPFS
      - +
      - Blockchain
  /ethledger/existsdoc:
    post:
      summary: Check document exists on blockchain
      description: Check if your documents exists in the eth blockchain
      operationId: EthledgerExistsdocPost
      x-api-path-slug: ethledgerexistsdoc-post
      parameters:
      - in: header
        name: ApiKey
      - in: formData
        name: files
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Check
      - Document
      - Exists
      - "On"
      - Blockchain
  /ethledger/docstatus:
    post:
      summary: Get document status with file
      description: Review the document status - existence, hash, block info, signatories,
        routing to users and details
      operationId: EthledgerDocstatusPost
      x-api-path-slug: ethledgerdocstatus-post
      parameters:
      - in: header
        name: ApiKey
      - in: formData
        name: files
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Document
      - Status
      - File
  /ethledger/sign:
    post:
      summary: Sign document
      description: Cryptographically sign the document and add the record to blockchain.  The
        document history and status is updated for querying.
      operationId: EthledgerSignPost
      x-api-path-slug: ethledgersign-post
      parameters:
      - in: header
        name: ApiKey
      - in: formData
        name: files
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Sign
      - Document
  /ethledger/sendforsign:
    post:
      summary: Send document
      description: Route the document for signature.  The document history and status
        is updated for querying.
      operationId: EthledgerSendforsignPost
      x-api-path-slug: ethledgersendforsign-post
      parameters:
      - in: header
        name: ApiKey
      - in: formData
        name: files
      - in: formData
        name: recipient
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Send
      - Document
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---