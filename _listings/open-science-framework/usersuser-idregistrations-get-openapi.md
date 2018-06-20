---
swagger: "2.0"
x-collection-name: Open Science Framework
x-complete: 0
info:
  title: Open Science Framework List all registrations
  description: |-
    A paginated list of registrations that the user is a contributor to. The returned registrations are sorted by their `date_modified`, with the most recently updated registrations appearing first.

    If the user ID in the path is the same as the logged-in user, all registrations will be returned. Otherwise, only the user's public registrations will be returned.

    User nodes are not available at this endpoint.
    #### Returns
    Returns a JSON object containing `data` and `links` keys.

    The `data` key contains an array of 10 registrations. Each resource in the array is a separate registration object and contains the full representation of the registration, meaning additional requests to a registration's detail view are not necessary.

    The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).
    #### Filtering
    You can optionally request that the response only include registrations that match your filters by utilizing the `filter` query parameter, e.g. https://api.osf.io/v2/users/cdi38/registrations/?filter[title]=replication.

    Registrations may be filtered by their `id`, `title`, `category`, `description`, `public`, `tags`, `date_created`, `date_modified`, `root`, `parent`, and `contributors`.
  contact:
    name: OSF
    url: https://osf.io/support
    email: support@osf.io
  version: "2.0"
host: test-api.osf.io
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /institutions/{institution_id}/registrations/:
    get:
      summary: List all affiliated registrations
      description: |-
        A paginated list of all registrations affiliated with an institution.
        #### Returns
        Returns a JSON object containing `data` and `links` keys.

        The `data` key contains an array of 10 registrations. Each resource in the array is a separate users object.

        The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).

        If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
        #### Filtering
        You can optionally request that the response only include registrations that match your filters by utilizing the `filter` query parameter, e.g. https://api.osf.io/v2/institutions/cos/registrations?filter[title]=science.

        Registrations may be filtered by their  `id`, `title`, `description`, `public`, `tags`, `category`, `date_created`, `date_modified`, `root`, `parent`, `contributors`, and `preprint`
      operationId: institutions_registration_list
      x-api-path-slug: institutionsinstitution-idregistrations-get
      parameters:
      - in: path
        name: institution_id
        description: The unique identifier of the institution you wish to retrieve
      responses:
        200:
          description: OK
      tags:
      - Institutions
      - Institution
      - Registrations
  /nodes/{node_id}/draft_registrations/:
    get:
      summary: List all draft registrations
      description: |-
        A paginated list of all of the draft registrations of a given node.

        Draft registrations contain the supplemental registration questions that accompany a registration. A registration is a frozen version of the project that can never be edited or deleted, but can be withdrawn.

        Your original project remains editable but will now have the draft registration linked to it.
        #### Permissions
        Only project administrators may view draft registrations.
        #### Returns
        Returns a JSON object containing `data` and `links` keys.

        The `data` key contains an array of 10 draft registrations. Each resource in the array is a separate draft registration object and contains the full representation of the draft registration, meaning additional requests to a draft registration's detail view are not necessary.

        The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).
      operationId: nodes_draft_registrations_list
      x-api-path-slug: nodesnode-iddraft-registrations-get
      parameters:
      - in: path
        name: node_id
        description: The unique identifier of the node
      responses:
        200:
          description: OK
      tags:
      - Nodes
      - Node
      - Draft
      - Registrations
    post:
      summary: Create a draft registration
      description: |-
        Initiate a draft registration of the current node.
        Draft registrations contain the supplemental registration questions that accompany a registration. A registration is a frozen version of the project that can never be edited or deleted, but can be withdrawn.

        Your original project remains editable but will now have the draft registration linked to it.
        #### Permissions
        Only project administrators may view create registrations.
        #### Required
        Required fields for creating a draft registration include:

        &nbsp;&nbsp;&nbsp;&nbsp`registration_supplement`
        #### Returns
        Returns a JSON object with a `data` key containing the representation of the created draft registration, if the request is successful.

        If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
      operationId: nodes_draft_registrations_create
      x-api-path-slug: nodesnode-iddraft-registrations-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: node_id
        description: The unique identifier of the node
      responses:
        200:
          description: OK
      tags:
      - Nodes
      - Node
      - Draft
      - Registrations
  /nodes/{node_id}/draft_registrations/{draft_id}/:
    delete:
      summary: Delete a draft registration
      description: |-
        Permanently deletes a draft registration. A draft that has already been registered cannot be deleted.
        #### Permissions
        Only project administrators may delete draft registrations.
        #### Returns
        If the request is successful, no content is returned.

        If the request is unsuccessful, a JSON object with an `errors` key containing information about the failure will be returned. Refer to the [list of error codes]() to understand why this request may have failed.
      operationId: nodes_draft_registrations_delete
      x-api-path-slug: nodesnode-iddraft-registrationsdraft-id-delete
      parameters:
      - in: path
        name: draft_id
        description: The unique identifier of the draft registration
      - in: path
        name: node_id
        description: The unique identifier of the node
      responses:
        200:
          description: OK
      tags:
      - Nodes
      - Node
      - Draft
      - Registrations
      - Draft
    get:
      summary: Retrieve a draft registration
      description: |-
        Retrieve the details of a given draft registration.
        Draft registrations contain the supplemental registration questions that accompany a registration. A registration is a frozen version of the project that can never be edited or deleted, but can be withdrawn.

        Your original project remains editable but will now have the draft registration linked to it.
        #### Permissions
        Only project administrators may view draft registrations.
        #### Returns
        Returns a JSON object with a `data` key containing the representation of the requested draft registration, if the request is successful.

        If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
      operationId: nodes_draft_registrations_read
      x-api-path-slug: nodesnode-iddraft-registrationsdraft-id-get
      parameters:
      - in: path
        name: draft_id
        description: The unique identifier of the draft registration
      - in: path
        name: node_id
        description: The unique identifier of the node
      responses:
        200:
          description: OK
      tags:
      - Nodes
      - Node
      - Draft
      - Registrations
      - Draft
    patch:
      summary: Update a draft registration
      description: |-
        Updates a draft registration by setting the values of the attributes specified in the request body. Any unspecified attributes will be left unchanged.

        Draft registrations contain the supplemental registration questions that accompany a registration. Answer the questions in the draft registration supplement by sending update requests until you are ready to submit the draft.

        The registration supplement of a draft registration cannot be updated after the draft has been created.

        When updating a draft registration, `registration_metadata` is required. It must be a dictionary with keys as question ids in the registration form, and values as nested dictionaries matching the specific format in the [registration schema](TODO: link me pls).

        If a question is multiple-choice, the question response must exactly match one of the possible choices.
        #### Permissions
        Only project administrators may update draft registrations.
        #### Returns
        Returns a JSON object with a `data` key containing the new representation of the updated draft registration, if the request is successful.

        If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
      operationId: nodes_draft_registrations_partial_update
      x-api-path-slug: nodesnode-iddraft-registrationsdraft-id-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: draft_id
        description: The unique identifier of the draft registration
      - in: path
        name: node_id
        description: The unique identifier of the node
      responses:
        200:
          description: OK
      tags:
      - Nodes
      - Node
      - Draft
      - Registrations
      - Draft
  /nodes/{node_id}/registrations/:
    get:
      summary: List all registrations
      description: |-
        List of all registrations of the given node.
        ####Returns

        Returns a JSON object containing `data` and `links` keys.

        The `data` key contains an array of up to 10 registrations. Each resource in the array is a separate registrations object.

        The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).
        ####Filtering

        You can optionally request that the response only include registrations that match your filters by utilizing the filter query parameter, e.g. https://api.osf.io/v2/registrations/?filter[title]=open.

        Registrations may be filtered by their `id`, `title`, `category`, `description`, `public`, `tags`, `date_created`, `date_modified`, `root`, `parent`, and `contributors`.
      operationId: nodes_registrations_list
      x-api-path-slug: nodesnode-idregistrations-get
      parameters:
      - in: path
        name: node_id
        description: The unique identifier of the node
      responses:
        200:
          description: OK
      tags:
      - Nodes
      - Node
      - Registrations
  /registrations/:
    get:
      summary: List all registrations
      description: |-
        A paginated list of registrations on the OSF to which the user has access.

        The returned registrations are those which are public or which the user has access to view.

        Non-registered nodes cannot be accessed through this endpoint (use the [nodes](#Nodes_nodes_list) endpoints instead).

        #### Registrations
        A registration on the OSF creates a frozen, time-stamped version of a project that cannot be edited or deleted. The *original project* can still be edited, while the registered version cannot.

        Registrations can be made public immediately or embargoed for up to 4 years.

        #### Withdrawals
        Registrations cannot be deleted, but they can be withdrawn. Withdrawing a registration removes the content of the registration but leaves behind basic metadata. A withdrawn registration will display a limited subset of information, namely, title, description, date_created, date_registered, date_withdrawn, registration, withdrawn, withdrawal_justification, and registration supplement. All other fields will be displayed as null. Additionally, the only relationship that remains accesible for a withdrawn registration is the contributors. All other relationships will return a **403 Forbidden** response.
        #### Returns
        Returns a JSON object containing `data` and `links` keys.

        The `data` key contains an array of 10 registrations. Each resource in the array is a separate registration object and contains the full representation of the registration, meaning additional requests to a registration's detail view are not necessary.

        The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).

        This request should never return an error.
        #### Filtering
        You can optionally request that the response only include registrations that match your filters by utilizing the `filter` query parameter, e.g. https://api.osf.io/v2/registrations/?filter[title]=open.

        Registrations may be filtered by their `id`, `title`, `category`, `description`, `public`, `tags`, `date_created`, `date_modified`, `root`, `parent`, and `contributors`.
      operationId: registrations_list
      x-api-path-slug: registrations-get
      responses:
        200:
          description: OK
      tags:
      - Registrations
  /registrations/{registration_id}/:
    get:
      summary: Retrieve a registration
      description: |-
        Retrieve the details of a given registration.
        #### Permissions
        Only project contributors may retrieve the details of a registration that is embargoed, or has not yet been made public. Attempting to retrieve a private registration for which you are not a contributor will result in a **403 Forbidden** response.

        Authentication is not required to view the details of a public registration, as public registrations give read-only access to everyone.
        #### Registrations
        A registration on the OSF creates a frozen, time-stamped version of a project that cannot be edited or deleted. The *original project* can still be edited, while the registered version cannot.

        Registrations can be made public immediately or embargoed for up to 4 years.

        #### Withdrawals
        Registrations cannot be deleted, but they can be withdrawn. Withdrawing a registration removes the content of the registration but leaves behind basic metadata. A withdrawn registration will display a limited subset of information, namely, title, description, date_created, date_registered, date_withdrawn, registration, withdrawn, withdrawal_justification, and registration supplement. All other fields will be displayed as null. Additionally, the only relationship that remains accesible for a withdrawn registration is the contributors. All other relationships will return a **403 Forbidden** response.
        #### Returns
        Returns a JSON object with a `data` key containing the representation of the requested registration, if the request is successful.

        If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
      operationId: registrations_read
      x-api-path-slug: registrationsregistration-id-get
      parameters:
      - in: path
        name: registration_id
        description: The unique identifier of the registration
      responses:
        200:
          description: OK
      tags:
      - Registrations
      - Registration
    patch:
      summary: Update a registration
      description: |-
        Updates a registration's privacy from **private** to **public**.

        Registrations can be updated with either a **PUT** or **PATCH** request. The `public` field is the only field that can be modified on a registration

        Registrations can only be turned from private to public, not vice versa.
        #### Permissions
        Only project administrators may update a registration.
        #### Returns
        Returns a JSON object with a `data` key containing the new representation of the updated registration, if the request is successful.

        If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
      operationId: registrations_partial_update
      x-api-path-slug: registrationsregistration-id-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: registration_id
        description: The unique identifier of the registration
      responses:
        200:
          description: OK
      tags:
      - Registrations
      - Registration
  /registrations/{registration_id}/children/:
    get:
      summary: List all child registrations
      description: |-
        A paginated list of children of a registration.

        The list consists of the next level child registrations for the given registration. The returned registrations are sorted by their `date_modified`, with the most recently updated child registrations appearing first.

        The list will include child registrations that are public, as well as child registrations that are private, if the authenticated user has permission to view them.
        #### Returns
        Returns a JSON object containing `data` and `links` keys.

        The `data` key contains an array of up to 10 child registrations. If the given registration has zero child registrations, the `data` key will contain an empty array. Each resource in the array is a separate registration object and contains the full representation of the child registration.

        The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).

        #### Filtering
        You can optionally request that the response only include registrations that match your filters by utilizing the `filter` query parameter, e.g. https://api.osf.io/v2/registrations/wucr8/children/?filter[title]=reproducibility.

        Registrations may be filtered by their `id`, `title`, `category`, `description`, `public`, `tags`, `date_created`, `date_modified`, `root`, `parent`, and `contributors`.

        Most fields are string fields and will be filtered using simple substring matching. Public is a boolean field, and can be filtered using truthy values, such as **true**, **false**, **0** or **1**. Note that quoting true or false in the query will cause the match to fail.
      operationId: registrations_children_list
      x-api-path-slug: registrationsregistration-idchildren-get
      parameters:
      - in: path
        name: registration_id
        description: The unique identifier of the registration
      responses:
        200:
          description: OK
      tags:
      - Registrations
      - Registration
      - Children
  /registrations/{registration_id}/citations/:
    get:
      summary: List all citation styles
      description: |-
        A paginated list of the registration's alternative citation styles

        #### Returns
        Returns a JSON object containing `data` and `links` keys.

        The `data` key contains an array of up to 10 citation styles. Each resource in the array is a separate citation styles object.

        The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).
        #### Filtering
        You can optionally request that the response only include citation styles that match your filters by utilizing the `filter` query parameter, e.g. https://api.osf.io/v2/registrations/wucr8/citations/?filter[title]=open.

        Citation styles may be filtered by their `id`, `title`, `short-title`, and `summary`.
      operationId: registrations_citations_list
      x-api-path-slug: registrationsregistration-idcitations-get
      parameters:
      - in: path
        name: registration_id
        description: The unique identifier of the registration
      responses:
        200:
          description: OK
      tags:
      - Registrations
      - Registration
      - Citations
  /registrations/{registration_id}/citations/{citation_id}/:
    get:
      summary: Retrieve a citation
      description: |-
        Retrieves the citation style details for a registration, in CSL format.
        #### Returns
        Returns a JSON object with a `data` key that contains the representation of the details necessary for the citation style.
      operationId: registrations_citation_read
      x-api-path-slug: registrationsregistration-idcitationscitation-id-get
      parameters:
      - in: path
        name: citation_id
        description: The unique identifier of the citation
      - in: path
        name: registration_id
        description: The unique identifier of the registration
      responses:
        200:
          description: OK
      tags:
      - Registrations
      - Registration
      - Citations
      - Citation
  /registrations/{registration_id}/comments/:
    get:
      summary: List all comments
      description: |-
        A paginated list of the registration's comments.

        The returned comments are sorted by their creation date, with the most recent comments appearing first.
        ####Permissions
        Comments of public registrations are given read-only access to everyone.

        If the comment-level is `private`, only registration contributors have permission to comment.

        If the comment-level is `public`, any logged-in OSF user can comment.

        Comments of private registrations are only visible to contributors and administrators on the registration.
        ####Returns
        Returns a JSON object containing `data` and `links` keys.

        The `data` key contains an array of comment objects. Each resource in the array is a separate comment object.

        The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).
        #### Filtering
        You can optionally request that the response only include comments that match your filters by utilizing the `filter` query parameter, e.g. https://api.osf.io/v2/registrations/wuerf/comments/?filter[target]=wuerf

        Comments may be filtered by their `deleted`, `target`, `date_created`, `date_modified`.

        Most fields are string fields and will be filtered using simple substring matching. Deleted is a boolean field, and can be filtered using truthy values, such as **true**, **false**, **0** or **1**. Note that quoting `true` or `false` in the query will cause the match to fail.
      operationId: registrations_comments_list
      x-api-path-slug: registrationsregistration-idcomments-get
      parameters:
      - in: path
        name: registration_id
        description: The unique identifier of the registration
      responses:
        200:
          description: OK
      tags:
      - Registrations
      - Registration
      - Comments
  /registrations/{registration_id}/contributors/:
    get:
      summary: List all contributors
      description: |-
        A paginated list of all contributors on this registration.
        The returned contributors are sorted by their index.

        Contributors are users who can make changes to the registration or, in the case of private registration, have read access to the registration.

        Contributors are categorized as either "bibliographic" or "non-bibliographic". From a permissions standpoint, both are the same, but bibliographic contributors are included in citations and are listed in the contributors list on the OSF, while non-bibliographic contributors are not.

        Note that if an anonymous view_only key is being used to view the list of contributors, the user relationship will not be exposed and the contributor ID will be an empty string.

        #### Returns
        Returns a JSON object containing `data` and `links` keys.

        The `data` key contains an array of up to 10 contributors. Each resource in the array contains the full representation of the contributor. Additionally, the full representation of the user this contributor represents is automatically embedded within the `data` key of the response.

        The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).
        #### Filtering
        You can optionally request that the response only include contributors that match your filters by utilizing the `filter` query parameter, e.g. https://api.osf.io/v2/registrations/wu3a4/contributors/?filter[bibliographic]=true.

        Contributors may be filtered by their `bibliographic` and `permission` attributes.
      operationId: registrations_contributors_list
      x-api-path-slug: registrationsregistration-idcontributors-get
      parameters:
      - in: path
        name: registration_id
        description: The unique identifier of the registration
      responses:
        200:
          description: OK
      tags:
      - Registrations
      - Registration
      - Contributors
  /registrations/{registration_id}/contributors/{user_id}/:
    get:
      summary: Retrieve a contributor
      description: |-
        Retrieves the details of a contributor on this registration.

        #### Returns
        Returns a JSON object with a `data` key containing the representation of the requested contributor, if the request is successful.

        If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
      operationId: registrations_contributors_read
      x-api-path-slug: registrationsregistration-idcontributorsuser-id-get
      parameters:
      - in: path
        name: registration_id
        description: The unique identifier of the registration
      - in: path
        name: user_id
        description: The unique identifier of the user
      responses:
        200:
          description: OK
      tags:
      - Registrations
      - Registration
      - Contributors
      - User
  /registrations/{registration_id}/files/:
    get:
      summary: List all storage providers
      description: |-
        A paginated list of storage providers enabled on the registration

        Users of the OSF may access their data on a [number of cloud-storage services](https://api.osf.io/v2/#storage-providers) that have integrations with the OSF. We call these **providers**. By default, every node has access to the OSF-provided storage but may use as many of the supported providers as desired.


        ####Returns
        Returns a JSON object containing `data` and `links` keys.

        The `data` key contains an array of up to 10 files. Each resource in the array is a separate file object.

        The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).

        Note: In the OSF filesystem model, providers are treated as folders, but with special properties that distinguish them from regular folders. Every provider folder is considered a root folder, and may not be deleted through the regular file API.
      operationId: registrations_providers_list
      x-api-path-slug: registrationsregistration-idfiles-get
      parameters:
      - in: path
        name: registration_id
        description: The unique identifier of the registration
      responses:
        200:
          description: OK
      tags:
      - Registrations
      - Registration
      - Files
  /registrations/{registration_id}/files/{provider}/:
    get:
      summary: List all files
      description: |-
        List of all the registration's files/folders for a given storage provider.

        ####Returns

        Returns a JSON object containing `data` and `links` keys.

        The `data` key contains an array of files. Each resource in the array is a separate file object and contains the full representation of the file.

        The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).

        ####Filtering

        You can optionally request that the response only include files that match your filters by utilizing the `filter` query parameter, e.g. https://api.osf.io/v2/registrations/wucr8/files/osfstorage/?filter[kind]=file

        Files may be filtered by `id`, `name`, `node`, `kind`, `path`, `provider`, `size`, and `last_touched`.
      operationId: registrations_files_list
      x-api-path-slug: registrationsregistration-idfilesprovider-get
      parameters:
      - in: path
        name: provider
        description: The unique identifier of the storage provider
      - in: path
        name: registration_id
        description: The unique identifier of the registration
      responses:
        200:
          description: OK
      tags:
      - Registrations
      - Registration
      - Files
      - Provider
  /registrations/{registration_id}/files/{provider}/{path}/:
    get:
      summary: Retrieve a file
      description: |-
        Retrieves the details of a registration file for the given storage provider.
        ####Returns
        Returns a JSON object with a `data` key containing the representation of the requested registration file object, if the request is successful.

        If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
      operationId: registrations_files_read
      x-api-path-slug: registrationsregistration-idfilesproviderpath-get
      parameters:
      - in: path
        name: path
        description: The unique identifier of the file path
      - in: path
        name: provider
        description: The unique identifier of the storage provider
      - in: path
        name: registration_id
        description: The unique identifier of the registration
      responses:
        200:
          description: OK
      tags:
      - Registrations
      - Registration
      - Files
      - Provider
      - Path
  /registrations/{registration_id}/forks/:
    get:
      summary: List all forks
      description: "A paginated list of the registration\u2019s forks\n\nThe returned
        forks are sorted by their `forked_date`, with the most recent forks appearing
        first.\n\nForking a registration creates a copy of an existing registration
        and all of its contents.\n#### Returns\nReturns a JSON object containing `data`
        and `links` keys.\n\nThe `data` key contains an array of up to 10 forks. If
        the current registration has no fork, the `data` key will contain an empty
        array. Each resource in the array is a separate registration object and contains
        the full representation of the registration's fork.\n\nThe `links` key contains
        a dictionary of links that can be used for [pagination](#Introduction_pagination)."
      operationId: registrations_forks_list
      x-api-path-slug: registrationsregistration-idforks-get
      parameters:
      - in: path
        name: registration_id
        description: The unique identifier of the registration
      responses:
        200:
          description: OK
      tags:
      - Registrations
      - Registration
      - Forks
    post:
      summary: Create a fork
      description: |-
        Creates a fork of the given registration.

        Forking a project creates a copy of an existing registration and all of its contents. The fork always points back to the original registration, forming a network of registrations.

        You might use a fork to copy another's work to build on and extend. For example, a professor may create an OSF project of materials for individual student use. Each student forks the project to have his or her own copy of the materials to start his/her own work.

        When creating a fork, your fork will only contain public components of the current registration and components for which you are a contributor. Private components that you do not have access to will not be forked.
        #### Required
        There are no required attributes when creating a fork, as all of the forked registration's attributes will be copied from the current registration.

        The `title` field is optional, with the default title being "Fork of " prepended to the current registration's title.
        #### Returns
        Returns a JSON object with a `data` key containing the complete representation of the forked registration, if the request is successful.
        If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
      operationId: registrations_forks_create
      x-api-path-slug: registrationsregistration-idforks-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: registration_id
        description: The unique identifier of the registration
      responses:
        200:
          description: OK
      tags:
      - Registrations
      - Registration
      - Forks
  /registrations/{registration_id}/identifiers/:
    get:
      summary: List all identifiers
      description: |-
        A paginated list of the registration's identifiers.
        ####Returns
        Returns a JSON object containing `data` and `links` keys.

        The `data` key contains an array of identifiers. Each resource in the array is a separate identifier object.

        The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).
        ####Filtering

        You can optionally request that the response only include registrations that match your filters by utilizing the `filter` query parameter, e.g. https://api.osf.io/v2/registrations/wucr8/identifiers/?filter[category]=ark

        Identifiers may be filtered by their `category` e.g `ark` or `doi`.
      operationId: registrations_identifiers_list
      x-api-path-slug: registrationsregistration-ididentifiers-get
      parameters:
      - in: path
        name: registration_id
        description: The unique identifier of the registration
      responses:
        200:
          description: OK
      tags:
      - Registrations
      - Registrationentifiers
  /registrations/{registration_id}/institutions/:
    get:
      summary: List all institutions
      description: |-
        A paginated list of institutions affiliated with the registration.
        ####Returns
        Returns a JSON object containing `data` and `links` keys.

        The `data` key contains an array of up to 10 affiliated institutions. Each resource in the array is a separate institution object.

        The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).
      operationId: registrations_institutions_list
      x-api-path-slug: registrationsregistration-idinstitutions-get
      parameters:
      - in: path
        name: registration_id
        description: The unique identifier of the registration
      responses:
        200:
          description: OK
      tags:
      - Registrations
      - Registration
      - Institutions
  /registrations/{registration_id}/linked_nodes/:
    get:
      summary: List all linked nodes
      description: |-
        List of all nodes linked to the registration.
        ####Returns
        Returns a JSON object containing `data` and `links` keys.

        The `data` key contains an array of up to 10 nodes. Each resource in the array is a separate node object.

        The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).
        ####Filtering
        You can optionally request that the response only include nodes that match your filters by utilizing the `filter` query parameter, e.g. https://api.osf.io/v2/registrations/wucr8/linked_nodes/?filter[title]=reproducibility/?filter[title]=reproducibility.

        Nodes may be filtered by their `title`, `category`, `description`, `public`, `registration`, or `tags`. `title`, `description`, and `category` are string fields and will be filteres using simple substring matching. `public`, `registration` are boolean and can be filtered using truthy values, such as `true`, `false`, `0`, `1`. `tags` is an array of simple strings.
      operationId: registrations_linked_nodes_list
      x-api-path-slug: registrationsregistration-idlinked-nodes-get
      parameters:
      - in: path
        name: registration_id
        description: The unique identifier of the registration
      responses:
        200:
          description: OK
      tags:
      - Registrations
      - Registration
      - Linked
      - Nodes
  /registrations/{registration_id}/logs/:
    get:
      summary: List all logs
      description: |-
        A paginated list of the registration's logs.

        The returned logs are sorted by their `date`, with the most recents logs appearing first.

        ####Returns
        Returns a JSON object containing `data` and `links` keys.

        The `data` key contains an array of up to 10 logs. Each resource in the array is a separate logs object.

        The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).
        ####Filtering
        You can optionally request that the response only include logs that match your filters by utilizing the `filter` query parameter, e.g. https://api.osf.io/v2/registrations/wucr8/logs/?filter[action]=made_private.

        Logs may be filtered by their `action`, and `date`.
      operationId: registrations_logs_list
      x-api-path-slug: registrationsregistration-idlogs-get
      parameters:
      - in: path
        name: registration_id
        description: The unique identifier of the registration
      responses:
        200:
          description: OK
      tags:
      - Registrations
      - Registration
      - Logs
  /registrations/{registration_id}/view_only_links/:
    get:
      summary: List all view only links
      description: |-
        A paginated list of view only links created for this registration.
        ####Returns
        Returns a JSON object containing `data` and `links` keys.

        The `data` key contains an array of up to 10 view only links. Each resource in the array is a view only link object.

        The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).

        ####Permissions

        View only links on a registration, public or private, are readable and writeable only by users that are administrators on the registration.

        ####Filtering

        You can optionally request that the response only include view only links that match your filters by utilizing the `filter` query parameter, e.g. https://api.osf.io/v2/registrations/wu3a4/view_only_links/?filter[anonymous]=true.

        View Only Links may be filtered based on their `name`, `anonymous` and `date_created` fields. Possible comparison operators include 'gt' (greater than), 'gte'(greater than or equal to), 'lt' (less than) and 'lte' (less than or equal to). The date must be in the format YYYY-MM-DD and the time is optional.
      operationId: registrations_view_only_links_list
      x-api-path-slug: registrationsregistration-idview-only-links-get
      parameters:
      - in: path
        name: registration_id
        description: The unique identifier of the registration
      responses:
        200:
          description: OK
      tags:
      - Registrations
      - Registration
      - View
      - Only
      - Links
  /registrations/{registration_id}/view_only_links/{link_id}/:
    get:
      summary: Retrieve a view only link
      description: |-
        Retrieves the details of a view only link created from this registration.
        ####Returns
        Returns a JSON object with a `data` key containing the representation of the requested view only link, if the request is successful.

        If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
        ####Permissions

        View only links on a registration, public or private, are readable and writeable only by users that are administrators on the registration.
      operationId: registrations_view_only_links_read
      x-api-path-slug: registrationsregistration-idview-only-linkslink-id-get
      parameters:
      - in: path
        name: link_id
        description: The unique identifier of the view only link
      - in: path
        name: registration_id
        description: The unique identifier of the registration
      responses:
        200:
          description: OK
      tags:
      - Registrations
      - Registration
      - View
      - Only
      - Links
      - Link
  /registrations/{registration_id}/wikis/:
    get:
      summary: List all wikis
      description: |-
        A paginated list of the registration's wiki pages
        ####Returns
        A list of all registration's current wiki page versions ordered by their date_modified. Each resource contains the full representation of the wiki, meaning additional requests to an individual wiki's detail view are not necessary.

        If the request is unsuccessful, a JSON object with an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
        #### Filtering
        Wiki pages can be filtered based on their `name` and `date_modified` fields.
        + `filter[name]=<Str>` -- filter wiki pages by name
        + `filter[date_modified][comparison_operator]=YYYY-MM-DDTH:M:S` -- filter wiki pages based on date modified.

        Possible comparison operators include 'gt' (greater than), 'gte'(greater than or equal to), 'lt' (less than) and 'lte' (less than or equal to). The date must be in the format YYYY-MM-DD and the time is optional.
      operationId: registrations_wikis_list
      x-api-path-slug: registrationsregistration-idwikis-get
      parameters:
      - in: path
        name: registration_id
        description: The unique identifier of the registration
      responses:
        200:
          description: OK
      tags:
      - Registrations
      - Registration
      - Wikis
  /users/{user_id}/registrations/:
    get:
      summary: List all registrations
      description: |-
        A paginated list of registrations that the user is a contributor to. The returned registrations are sorted by their `date_modified`, with the most recently updated registrations appearing first.

        If the user ID in the path is the same as the logged-in user, all registrations will be returned. Otherwise, only the user's public registrations will be returned.

        User nodes are not available at this endpoint.
        #### Returns
        Returns a JSON object containing `data` and `links` keys.

        The `data` key contains an array of 10 registrations. Each resource in the array is a separate registration object and contains the full representation of the registration, meaning additional requests to a registration's detail view are not necessary.

        The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).
        #### Filtering
        You can optionally request that the response only include registrations that match your filters by utilizing the `filter` query parameter, e.g. https://api.osf.io/v2/users/cdi38/registrations/?filter[title]=replication.

        Registrations may be filtered by their `id`, `title`, `category`, `description`, `public`, `tags`, `date_created`, `date_modified`, `root`, `parent`, and `contributors`.
      operationId: users_registrations_list
      x-api-path-slug: usersuser-idregistrations-get
      parameters:
      - in: path
        name: user_id
        description: The unique identifier of the user
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Registrations
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