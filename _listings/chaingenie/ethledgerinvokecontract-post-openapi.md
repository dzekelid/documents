---
swagger: "2.0"
x-collection-name: ChainGenie
x-complete: 0
info:
  title: ChainGenie Generate, Sign & Route Document (Advanced)
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
  /ethledger/docert:
    post:
      summary: Generate and Manage Document (Basic)
      description: "This is an over simplified version for testing this API for its
        powers a template - uses an inbuilt into ChainGenie template and values are
        preconfigured - just running this will work and provide you an IPFS handle
        to retrieve the document you generated with your variables / values from the
        template.\nUse an existing document on our server and generate a document
        with automated sign and routing to a recipient.  Ex. this configured api will
        generate a certificate for a student name (name) with the completed certificate
        course (course) and dated (date). \nThe document hash will be posted on blockchain
        and the actual document will be added to IPFS.  Want to retrieve your document?
        Check out the API - Write & Retrieve - Docs (IPFS)."
      operationId: EthledgerDocertPost2
      x-api-path-slug: ethledgerdocert-post
      parameters:
      - in: header
        name: ApiKey
      - in: formData
        name: course
      - in: formData
        name: date
      - in: formData
        name: students
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Generate
      - Manage
      - Document
      - (Basic)
  /ethledger/invokecontract:
    post:
      summary: Generate, Sign & Route Document (Advanced)
      description: "This API is the generic version of the \"Generate document from
        template\" API. Any template file can be uploaded (sample available as link
        for testing).  If you just want to see how this would work - use the other
        call and just run it without any uploaded certificate. \nUpload a templated
        pdf with editable / filable fields and generate a document with automated
        sign and routing to a recipient.  Every attribute that needs to be filled
        will need to be passed in the format - ex. course field to be substituted
        - field = attrib; value = [\"course\",\"course value\"] or date field to be
        substituted - field = attrib; value = [\"date\",\"12/12/2016\"].  If your
        fillable form has the field named \"today\", current time will be used for
        filling the value of that field.\nYou will need to upload for the file attribute
        a real template file with fillable fields. For the sample values as configured,
        you can use the demo template available at http://chaingenie.com/cert.pdf.
        \ Download this certificate and add it as your input file\nTo route the document
        to recipient (optional) add field recipient with \"key\" of the recipient
        - available recipient in the system - 0xb3A214341df9560a3e09E256BfacefD6648f5Ca9
        for your testing\nUse case - Upload an invoice template with fillable fields,
        add attrib values for all the fields that needs to be filled, add the recipient
        field - your invoice will be created, signed with your key (in production
        / in test it will be signed with the local admin key) and will be routed to
        the recipient (in production you can add your recipient / in sandbox - use
        recipient 0xb3A214341df9560a3e09E256BfacefD6648f5Ca9)\nResponse will contain
        the document name, signatories, timestamps, recipient, IPFS hash (handle to
        retrieve the actual document)\nThe document hash will be posted on blockchain
        and the actual document will be added to IPFS.  Want to retrieve your document?
        Check out the API - Write & Retrieve - Docs (IPFS)."
      operationId: EthledgerInvokecontractPost
      x-api-path-slug: ethledgerinvokecontract-post
      parameters:
      - in: header
        name: ApiKey
      - in: formData
        name: attribs
      - in: formData
        name: file
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Generate
      - ""
      - Sign
      - '&'
      - Route
      - Document
      - (Advanced)
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