---
name: Open Science Framework
x-slug: open-science-framework
description: OSF provides free and open source project management support for researchers
  across the entire research lifecycle. As a collaboration tool, OSF helps researchers
  work on projects privately with a limited number of collaborators and make parts
  of their projects public, or make all the project publicly accessible for broader
  dissemination. As a workflow system, OSF enables connections to the many services
  researchers already use to streamline their process and increase efficiency. As
  a flexible repository, it can store and archive research data, protocols, and materials.
image: ""
x-kinRank: "7"
x-alexaRank: "0"
tags: Registrations
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/open-science-framework/apis.md
specificationVersion: "0.14"
apis:
- name: Open Science Framework List all affiliated registrations
  x-api-slug: open-science-framework
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
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2//institutions/{institution_id}/registrations/
  tags: Institutions,Institution,Registrations
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/open-science-framework/institutionsinstitution-idregistrations-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/open-science-framework/institutionsinstitution-idregistrations-get-openapi.md
- name: Open Science Framework List all draft registrations
  x-api-slug: open-science-framework
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
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2//nodes/{node_id}/draft_registrations/
  tags: Nodes,Node,Draft,Registrations
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/open-science-framework/nodesnode-iddraft-registrations-get-openapi.md
- name: Open Science Framework Create a draft registration
  x-api-slug: open-science-framework
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
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2//nodes/{node_id}/draft_registrations/
  tags: Nodes,Node,Draft,Registrations
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/open-science-framework/nodesnode-iddraft-registrations-post-openapi.md
- name: Open Science Framework Delete a draft registration
  x-api-slug: open-science-framework
  description: |-
    Permanently deletes a draft registration. A draft that has already been registered cannot be deleted.
    #### Permissions
    Only project administrators may delete draft registrations.
    #### Returns
    If the request is successful, no content is returned.

    If the request is unsuccessful, a JSON object with an `errors` key containing information about the failure will be returned. Refer to the [list of error codes]() to understand why this request may have failed.
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2//nodes/{node_id}/draft_registrations/{draft_id}/
  tags: Nodes,Node,Draft,Registrations,Draft
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/open-science-framework/nodesnode-iddraft-registrationsdraft-id-delete-openapi.md
- name: Open Science Framework Retrieve a draft registration
  x-api-slug: open-science-framework
  description: |-
    Retrieve the details of a given draft registration.
    Draft registrations contain the supplemental registration questions that accompany a registration. A registration is a frozen version of the project that can never be edited or deleted, but can be withdrawn.

    Your original project remains editable but will now have the draft registration linked to it.
    #### Permissions
    Only project administrators may view draft registrations.
    #### Returns
    Returns a JSON object with a `data` key containing the representation of the requested draft registration, if the request is successful.

    If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2//nodes/{node_id}/draft_registrations/{draft_id}/
  tags: Nodes,Node,Draft,Registrations,Draft
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/open-science-framework/nodesnode-iddraft-registrationsdraft-id-get-openapi.md
- name: Open Science Framework Update a draft registration
  x-api-slug: open-science-framework
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
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2//nodes/{node_id}/draft_registrations/{draft_id}/
  tags: Nodes,Node,Draft,Registrations,Draft
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/open-science-framework/nodesnode-iddraft-registrationsdraft-id-patch-openapi.md
- name: Open Science Framework List all registrations
  x-api-slug: open-science-framework
  description: |-
    List of all registrations of the given node.
    ####Returns

    Returns a JSON object containing `data` and `links` keys.

    The `data` key contains an array of up to 10 registrations. Each resource in the array is a separate registrations object.

    The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).
    ####Filtering

    You can optionally request that the response only include registrations that match your filters by utilizing the filter query parameter, e.g. https://api.osf.io/v2/registrations/?filter[title]=open.

    Registrations may be filtered by their `id`, `title`, `category`, `description`, `public`, `tags`, `date_created`, `date_modified`, `root`, `parent`, and `contributors`.
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2//nodes/{node_id}/registrations/
  tags: Nodes,Node,Registrations
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/open-science-framework/nodesnode-idregistrations-get-openapi.md
- name: Open Science Framework List all registrations
  x-api-slug: open-science-framework
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
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2//registrations/
  tags: Registrations
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/open-science-framework/registrations-get-openapi.md
- name: Open Science Framework Retrieve a registration
  x-api-slug: open-science-framework
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
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2//registrations/{registration_id}/
  tags: Registrations,Registration
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/open-science-framework/registrationsregistration-id-get-openapi.md
- name: Open Science Framework Update a registration
  x-api-slug: open-science-framework
  description: |-
    Updates a registration's privacy from **private** to **public**.

    Registrations can be updated with either a **PUT** or **PATCH** request. The `public` field is the only field that can be modified on a registration

    Registrations can only be turned from private to public, not vice versa.
    #### Permissions
    Only project administrators may update a registration.
    #### Returns
    Returns a JSON object with a `data` key containing the new representation of the updated registration, if the request is successful.

    If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2//registrations/{registration_id}/
  tags: Registrations,Registration
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/open-science-framework/registrationsregistration-id-patch-openapi.md
- name: Open Science Framework List all child registrations
  x-api-slug: open-science-framework
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
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2//registrations/{registration_id}/children/
  tags: Registrations,Registration,Children
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/open-science-framework/registrationsregistration-idchildren-get-openapi.md
- name: Open Science Framework List all citation styles
  x-api-slug: open-science-framework
  description: |-
    A paginated list of the registration's alternative citation styles

    #### Returns
    Returns a JSON object containing `data` and `links` keys.

    The `data` key contains an array of up to 10 citation styles. Each resource in the array is a separate citation styles object.

    The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).
    #### Filtering
    You can optionally request that the response only include citation styles that match your filters by utilizing the `filter` query parameter, e.g. https://api.osf.io/v2/registrations/wucr8/citations/?filter[title]=open.

    Citation styles may be filtered by their `id`, `title`, `short-title`, and `summary`.
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2//registrations/{registration_id}/citations/
  tags: Registrations,Registration,Citations
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/open-science-framework/registrationsregistration-idcitations-get-openapi.md
- name: Open Science Framework Retrieve a citation
  x-api-slug: open-science-framework
  description: |-
    Retrieves the citation style details for a registration, in CSL format.
    #### Returns
    Returns a JSON object with a `data` key that contains the representation of the details necessary for the citation style.
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2//registrations/{registration_id}/citations/{citation_id}/
  tags: Registrations,Registration,Citations,Citation
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/open-science-framework/registrationsregistration-idcitationscitation-id-get-openapi.md
- name: Open Science Framework List all comments
  x-api-slug: open-science-framework
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
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2//registrations/{registration_id}/comments/
  tags: Registrations,Registration,Comments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/open-science-framework/registrationsregistration-idcomments-get-openapi.md
- name: Open Science Framework List all contributors
  x-api-slug: open-science-framework
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
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2//registrations/{registration_id}/contributors/
  tags: Registrations,Registration,Contributors
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/open-science-framework/registrationsregistration-idcontributors-get-openapi.md
- name: Open Science Framework Retrieve a contributor
  x-api-slug: open-science-framework
  description: |-
    Retrieves the details of a contributor on this registration.

    #### Returns
    Returns a JSON object with a `data` key containing the representation of the requested contributor, if the request is successful.

    If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2//registrations/{registration_id}/contributors/{user_id}/
  tags: Registrations,Registration,Contributors,User
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/open-science-framework/registrationsregistration-idcontributorsuser-id-get-openapi.md
- name: Open Science Framework List all storage providers
  x-api-slug: open-science-framework
  description: |-
    A paginated list of storage providers enabled on the registration

    Users of the OSF may access their data on a [number of cloud-storage services](https://api.osf.io/v2/#storage-providers) that have integrations with the OSF. We call these **providers**. By default, every node has access to the OSF-provided storage but may use as many of the supported providers as desired.


    ####Returns
    Returns a JSON object containing `data` and `links` keys.

    The `data` key contains an array of up to 10 files. Each resource in the array is a separate file object.

    The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).

    Note: In the OSF filesystem model, providers are treated as folders, but with special properties that distinguish them from regular folders. Every provider folder is considered a root folder, and may not be deleted through the regular file API.
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2//registrations/{registration_id}/files/
  tags: Registrations,Registration,Files
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/open-science-framework/registrationsregistration-idfiles-get-openapi.md
- name: Open Science Framework List all files
  x-api-slug: open-science-framework
  description: |-
    List of all the registration's files/folders for a given storage provider.

    ####Returns

    Returns a JSON object containing `data` and `links` keys.

    The `data` key contains an array of files. Each resource in the array is a separate file object and contains the full representation of the file.

    The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).

    ####Filtering

    You can optionally request that the response only include files that match your filters by utilizing the `filter` query parameter, e.g. https://api.osf.io/v2/registrations/wucr8/files/osfstorage/?filter[kind]=file

    Files may be filtered by `id`, `name`, `node`, `kind`, `path`, `provider`, `size`, and `last_touched`.
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2//registrations/{registration_id}/files/{provider}/
  tags: Registrations,Registration,Files,Provider
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/open-science-framework/registrationsregistration-idfilesprovider-get-openapi.md
- name: Open Science Framework Retrieve a file
  x-api-slug: open-science-framework
  description: |-
    Retrieves the details of a registration file for the given storage provider.
    ####Returns
    Returns a JSON object with a `data` key containing the representation of the requested registration file object, if the request is successful.

    If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2//registrations/{registration_id}/files/{provider}/{path}/
  tags: Registrations,Registration,Files,Provider,Path
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/open-science-framework/registrationsregistration-idfilesproviderpath-get-openapi.md
- name: Open Science Framework List all forks
  x-api-slug: open-science-framework
  description: "A paginated list of the registration\u2019s forks\n\nThe returned
    forks are sorted by their `forked_date`, with the most recent forks appearing
    first.\n\nForking a registration creates a copy of an existing registration and
    all of its contents.\n#### Returns\nReturns a JSON object containing `data` and
    `links` keys.\n\nThe `data` key contains an array of up to 10 forks. If the current
    registration has no fork, the `data` key will contain an empty array. Each resource
    in the array is a separate registration object and contains the full representation
    of the registration's fork.\n\nThe `links` key contains a dictionary of links
    that can be used for [pagination](#Introduction_pagination)."
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2//registrations/{registration_id}/forks/
  tags: Registrations,Registration,Forks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/open-science-framework/registrationsregistration-idforks-get-openapi.md
- name: Open Science Framework Create a fork
  x-api-slug: open-science-framework
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
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2//registrations/{registration_id}/forks/
  tags: Registrations,Registration,Forks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/open-science-framework/registrationsregistration-idforks-post-openapi.md
- name: Open Science Framework List all identifiers
  x-api-slug: open-science-framework
  description: |-
    A paginated list of the registration's identifiers.
    ####Returns
    Returns a JSON object containing `data` and `links` keys.

    The `data` key contains an array of identifiers. Each resource in the array is a separate identifier object.

    The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).
    ####Filtering

    You can optionally request that the response only include registrations that match your filters by utilizing the `filter` query parameter, e.g. https://api.osf.io/v2/registrations/wucr8/identifiers/?filter[category]=ark

    Identifiers may be filtered by their `category` e.g `ark` or `doi`.
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2//registrations/{registration_id}/identifiers/
  tags: Registrations,Registrationentifiers
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/open-science-framework/registrationsregistration-ididentifiers-get-openapi.md
- name: Open Science Framework List all institutions
  x-api-slug: open-science-framework
  description: |-
    A paginated list of institutions affiliated with the registration.
    ####Returns
    Returns a JSON object containing `data` and `links` keys.

    The `data` key contains an array of up to 10 affiliated institutions. Each resource in the array is a separate institution object.

    The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2//registrations/{registration_id}/institutions/
  tags: Registrations,Registration,Institutions
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/open-science-framework/registrationsregistration-idinstitutions-get-openapi.md
- name: Open Science Framework List all linked nodes
  x-api-slug: open-science-framework
  description: |-
    List of all nodes linked to the registration.
    ####Returns
    Returns a JSON object containing `data` and `links` keys.

    The `data` key contains an array of up to 10 nodes. Each resource in the array is a separate node object.

    The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).
    ####Filtering
    You can optionally request that the response only include nodes that match your filters by utilizing the `filter` query parameter, e.g. https://api.osf.io/v2/registrations/wucr8/linked_nodes/?filter[title]=reproducibility/?filter[title]=reproducibility.

    Nodes may be filtered by their `title`, `category`, `description`, `public`, `registration`, or `tags`. `title`, `description`, and `category` are string fields and will be filteres using simple substring matching. `public`, `registration` are boolean and can be filtered using truthy values, such as `true`, `false`, `0`, `1`. `tags` is an array of simple strings.
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2//registrations/{registration_id}/linked_nodes/
  tags: Registrations,Registration,Linked,Nodes
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/open-science-framework/registrationsregistration-idlinked-nodes-get-openapi.md
- name: Open Science Framework List all logs
  x-api-slug: open-science-framework
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
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2//registrations/{registration_id}/logs/
  tags: Registrations,Registration,Logs
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/open-science-framework/registrationsregistration-idlogs-get-openapi.md
- name: Open Science Framework List all view only links
  x-api-slug: open-science-framework
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
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2//registrations/{registration_id}/view_only_links/
  tags: Registrations,Registration,View,Only,Links
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/open-science-framework/registrationsregistration-idview-only-links-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/open-science-framework/registrationsregistration-idview-only-links-get-openapi.md
- name: Open Science Framework Retrieve a view only link
  x-api-slug: open-science-framework
  description: |-
    Retrieves the details of a view only link created from this registration.
    ####Returns
    Returns a JSON object with a `data` key containing the representation of the requested view only link, if the request is successful.

    If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
    ####Permissions

    View only links on a registration, public or private, are readable and writeable only by users that are administrators on the registration.
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2//registrations/{registration_id}/view_only_links/{link_id}/
  tags: Registrations,Registration,View,Only,Links,Link
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/open-science-framework/registrationsregistration-idview-only-linkslink-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/open-science-framework/registrationsregistration-idview-only-linkslink-id-get-openapi.md
- name: Open Science Framework List all wikis
  x-api-slug: open-science-framework
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
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2//registrations/{registration_id}/wikis/
  tags: Registrations,Registration,Wikis
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/open-science-framework/registrationsregistration-idwikis-get-openapi.md
- name: Open Science Framework List all registrations
  x-api-slug: open-science-framework
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
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2//users/{user_id}/registrations/
  tags: Users,User,Registrations
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/open-science-framework/usersuser-idregistrations-get-openapi.md
- name: Open Science Framework
  x-api-slug: open-science-framework
  description: OSF provides free and open source project management support for researchers
    across the entire research lifecycle. As a collaboration tool, OSF helps researchers
    work on projects privately with a limited number of collaborators and make parts
    of their projects public, or make all the project publicly accessible for broader
    dissemination. As a workflow system, OSF enables connections to the many services
    researchers already use to streamline their process and increase efficiency. As
    a flexible repository, it can store and archive research data, protocols, and
    materials.
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2
  tags: Registrations
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/open-science-framework/openapi.md
x-common:
- type: x-website
  url: https://cos.io
- type: x-github
  url: https://github.com/OSFramework
- type: x-twitter
  url: https://twitter.com/OSFramework
- type: x-website
  url: http://osf.io
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---