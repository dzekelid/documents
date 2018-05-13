---
swagger: "2.0"
info:
  title: Box Update Folder, Create Shared Link, Create or Delete
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
  version: 1.0.0
host: api.box.com
basePath: /2.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /folders/{FOLDER_ID}:
    put:
      summary: Update Folder, Create Shared Link, Create or Delete
      description: Used to update information about the folder
      operationId: updateFolder
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: fields
        description: Attribute(s) to include in the response
      - in: path
        name: FOLDER_ID
      - in: header
        name: If-Match
        description: "This is in the \u2018etag\u2019 field of the folder object"
      responses:
        200:
          description: OK
      tags:
      - documents
      - folders
      - folder
definitions:
  Error:
    properties:
      type:
        description: This is a default description.
        type: delete
      status:
        description: This is a default description.
        type: delete
      context_info:
        description: This is a default description.
        type: delete
      code:
        description: This is a default description.
        type: delete
      help-url:
        description: This is a default description.
        type: delete
      message:
        description: This is a default description.
        type: delete
      request_id:
        description: This is a default description.
        type: delete
  Reference:
    properties:
      id:
        description: This is a default description.
        type: delete
      type:
        description: This is a default description.
        type: delete
  Pagination:
    properties:
      total_count:
        description: This is a default description.
        type: delete
      limit:
        description: This is a default description.
        type: delete
      offset:
        description: This is a default description.
        type: delete
      order:
        description: This is a default description.
        type: delete
  MarkerPagination:
    properties:
      limit:
        description: This is a default description.
        type: delete
      next_marker:
        description: This is a default description.
        type: delete
      prev_marker:
        description: This is a default description.
        type: delete
  ChunkPagination:
    properties:
      chunk_size:
        description: This is a default description.
        type: delete
      next_stream_position:
        description: This is a default description.
        type: delete
  UserReference:
    properties:
      type:
        description: This is a default description.
        type: delete
      id:
        description: This is a default description.
        type: delete
      name:
        description: This is a default description.
        type: delete
      login:
        description: This is a default description.
        type: delete
  FolderUploadEmail:
    properties:
      access:
        description: This is a default description.
        type: delete
      email:
        description: This is a default description.
        type: delete
  FolderPermissions:
    properties:
      can_download:
        description: This is a default description.
        type: delete
      can_upload:
        description: This is a default description.
        type: delete
      can_rename:
        description: This is a default description.
        type: delete
      cand_delete:
        description: This is a default description.
        type: delete
      can_share:
        description: This is a default description.
        type: delete
      can_invite_collaborator:
        description: This is a default description.
        type: delete
      can_set_share_access:
        description: This is a default description.
        type: delete
  FilePermissions:
    properties:
      can_download:
        description: This is a default description.
        type: delete
      can_preview:
        description: This is a default description.
        type: delete
      can_upload:
        description: This is a default description.
        type: delete
      can_rename:
        description: This is a default description.
        type: delete
      cand_delete:
        description: This is a default description.
        type: delete
      can_share:
        description: This is a default description.
        type: delete
      can_invite_collaborator:
        description: This is a default description.
        type: delete
      can_set_share_access:
        description: This is a default description.
        type: delete
  CopyFile:
    properties:
      parent:
        description: This is a default description.
        type: delete
      version:
        description: This is a default description.
        type: delete
      name:
        description: This is a default description.
        type: delete
  SharedLinkPermissions:
    properties:
      can_download:
        description: This is a default description.
        type: delete
      can_preview:
        description: This is a default description.
        type: delete
  SharedLink:
    properties:
      url:
        description: This is a default description.
        type: delete
      download_url:
        description: This is a default description.
        type: delete
      password:
        description: This is a default description.
        type: delete
      vanity_url:
        description: This is a default description.
        type: delete
      is_password_enabled:
        description: This is a default description.
        type: delete
      unshared_at:
        description: This is a default description.
        type: delete
      download_count:
        description: This is a default description.
        type: delete
      preview_count:
        description: This is a default description.
        type: delete
      access:
        description: This is a default description.
        type: delete
      effective_access:
        description: This is a default description.
        type: delete
  TemplateFields:
    properties:
      type:
        description: This is a default description.
        type: delete
      key:
        description: This is a default description.
        type: delete
      displayName:
        description: This is a default description.
        type: delete
      description:
        description: This is a default description.
        type: delete
      hidden:
        description: This is a default description.
        type: delete
      options:
        description: This is a default description.
        type: delete
  MetadataTemplate:
    properties:
      templateKey:
        description: This is a default description.
        type: delete
      scope:
        description: This is a default description.
        type: delete
      displayName:
        description: This is a default description.
        type: delete
      hidden:
        description: This is a default description.
        type: delete
      fields:
        description: This is a default description.
        type: delete
  WatermarkReference:
    properties:
      created_at:
        description: This is a default description.
        type: delete
      modified_at:
        description: This is a default description.
        type: delete
      imprint:
        description: This is a default description.
        type: delete
  Watermark:
    properties: []
  Event:
    properties:
      type:
        description: This is a default description.
        type: delete
      event_id:
        description: This is a default description.
        type: delete
      event_type:
        description: This is a default description.
        type: delete
      session_id:
        description: This is a default description.
        type: delete
      source:
        description: This is a default description.
        type: delete
      additional_details:
        description: This is a default description.
        type: delete
  RealtimeServer:
    properties:
      type:
        description: This is a default description.
        type: delete
      url:
        description: This is a default description.
        type: delete
      ttl:
        description: This is a default description.
        type: delete
      max_retries:
        description: This is a default description.
        type: delete
      retry_timeout:
        description: This is a default description.
        type: delete
  RetentionPolicyList:
    properties:
      entries:
        description: This is a default description.
        type: delete
  RetentionPolicyAssignmentList:
    properties:
      entries:
        description: This is a default description.
        type: delete
  AssignmentCounts:
    properties:
      user:
        description: This is a default description.
        type: delete
      folder:
        description: This is a default description.
        type: delete
      file:
        description: This is a default description.
        type: delete
      file_version:
        description: This is a default description.
        type: delete
  CreateTaskAssignment:
    properties: []
  InviteUser:
    properties: []
  CreateLegalHoldPolicyAssignment:
    properties:
      policy_id:
        description: This is a default description.
        type: delete
  CreateRetentionPolicyAssignment:
    properties:
      policy_id:
        description: This is a default description.
        type: delete
x-collection-name: Box
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