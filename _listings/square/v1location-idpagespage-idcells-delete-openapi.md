---
swagger: "2.0"
x-collection-name: Square
x-complete: 0
info:
  title: Square Connect API Deletes a cell from a Favorites page in Square Register.
  description: Deletes a cell from a Favorites page in Square Register.
  termsOfService: https://connect.squareup.com/tos
  contact:
    name: Square Developer Platform
    url: https://squareup.com/developers
    email: developers@squareup.com
  version: "2.0"
host: connect.squareup.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/{location_id}/items/{item_id}/fees/{fee_id}:
    delete:
      summary: Removes a fee assocation from an item, meaning the fee is no longer
        automatically applied to the item in Square Register.
      description: Removes a fee assocation from an item, meaning the fee is no longer
        automatically applied to the item in Square Register.
      operationId: RemoveFee
      x-api-path-slug: v1location-iditemsitem-idfeesfee-id-delete
      parameters:
      - in: path
        name: fee_id
        description: The ID of the fee to apply
      - in: path
        name: item_id
        description: The ID of the item to add the fee to
      - in: path
        name: location_id
        description: The ID of the fees associated location
      responses:
        200:
          description: OK
      tags:
      - Removes
      - Fee
      - Assocation
      - From
      - Item
      - ""
      - Meaning
      - Fee
      - Is
      - "No"
      - Longer
      - Automatically
      - Applied
      - To
      - Item
      - In
      - Square
      - Register
    put:
      summary: Associates a fee with an item, meaning the fee is automatically applied
        to the item in Square Register.
      description: Associates a fee with an item, meaning the fee is automatically
        applied to the item in Square Register.
      operationId: ApplyFee
      x-api-path-slug: v1location-iditemsitem-idfeesfee-id-put
      parameters:
      - in: path
        name: fee_id
        description: The ID of the fee to apply
      - in: path
        name: item_id
        description: The ID of the item to add the fee to
      - in: path
        name: location_id
        description: The ID of the fees associated location
      responses:
        200:
          description: OK
      tags:
      - Associates
      - Fee
      - Item
      - ""
      - Meaning
      - Fee
      - Is
      - Automatically
      - Applied
      - To
      - Item
      - In
      - Square
      - Register
  /v1/{location_id}/pages:
    get:
      summary: Lists all of a location's Favorites pages in Square Register.
      description: Lists all of a location's Favorites pages in Square Register.
      operationId: ListPages
      x-api-path-slug: v1location-idpages-get
      parameters:
      - in: path
        name: location_id
        description: The ID of the location to list Favorites pages for
      responses:
        200:
          description: OK
      tags:
      - Lists
      - ""
      - Of
      - Locations
      - Favorites
      - Pages
      - In
      - Square
      - Register
    post:
      summary: Creates a Favorites page in Square Register.
      description: Creates a Favorites page in Square Register.
      operationId: CreatePage
      x-api-path-slug: v1location-idpages-post
      parameters:
      - in: body
        name: body
        description: An object containing the fields to POST for the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: location_id
        description: The ID of the location to create an item for
      responses:
        200:
          description: OK
      tags:
      - Creates
      - Favorites
      - Page
      - In
      - Square
      - Register
  /v1/{location_id}/pages/{page_id}:
    put:
      summary: Modifies the details of a Favorites page in Square Register.
      description: Modifies the details of a Favorites page in Square Register.
      operationId: UpdatePage
      x-api-path-slug: v1location-idpagespage-id-put
      parameters:
      - in: body
        name: body
        description: An object containing the fields to POST for the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: location_id
        description: The ID of the Favorites pages associated location
      - in: path
        name: page_id
        description: The ID of the page to modify
      responses:
        200:
          description: OK
      tags:
      - Modifies
      - Details
      - Of
      - Favorites
      - Page
      - In
      - Square
      - Register
  /v1/{location_id}/pages/{page_id}/cells:
    delete:
      summary: Deletes a cell from a Favorites page in Square Register.
      description: Deletes a cell from a Favorites page in Square Register.
      operationId: DeletePageCell
      x-api-path-slug: v1location-idpagespage-idcells-delete
      parameters:
      - in: query
        name: column
        description: The column of the cell to clear
      - in: path
        name: location_id
        description: The ID of the Favorites pages associated location
      - in: path
        name: page_id
        description: The ID of the page to delete
      - in: query
        name: row
        description: The row of the cell to clear
      responses:
        200:
          description: OK
      tags:
      - S
      - Cell
      - From
      - Favorites
      - Page
      - In
      - Square
      - Register
    put:
      summary: Modifies a cell of a Favorites page in Square Register.
      description: Modifies a cell of a Favorites page in Square Register.
      operationId: UpdatePageCell
      x-api-path-slug: v1location-idpagespage-idcells-put
      parameters:
      - in: body
        name: body
        description: An object containing the fields to POST for the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: location_id
        description: The ID of the Favorites pages associated location
      - in: path
        name: page_id
        description: The ID of the page the cell belongs to
      responses:
        200:
          description: OK
      tags:
      - Modifies
      - Cell
      - Of
      - Favorites
      - Page
      - In
      - Square
      - Register
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