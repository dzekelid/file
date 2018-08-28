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
tags: File
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/file/master/_listings/open-science-framework/apis.md
specificationVersion: "0.14"
apis:
- name: Open Science Framework - Retrieve a file
  x-api-slug: filesfile-id-get
  description: |-
    Retrieves the details of a file (or folder)
    ####Returns
    Returns a JSON object with a `data` key containing the representation of the requested file, if the request was successful.

    If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
    ###Waterbutler API actions

    Files can be modified through the Waterbutler API routes found in `links` (`new_folder`, `move`, `upload`, `download`, and `delete`).

    #### Download (files)

    To download a file, issue a GET request against the download link. The response will have the Content-Disposition header set, which will will trigger a download in a browser.

    #### Create Subfolder (folders)

    You can create a subfolder of an existing folder by issuing a PUT request against the new_folder link. The ?kind=folder portion of the query parameter is already included in the new_folder link. The name of the new subfolder should be provided in the name query parameter. The response will contain a WaterButler folder entity. If a folder with that name already exists in the parent directory, the server will return a 409 Conflict error response.

    #### Upload New File (folders)


      To upload a file to a folder, issue a PUT request to the folder's upload link with the raw file data in the request body, and the kind and name query parameters set to 'file' and the desired name of the file. The response will contain a WaterButler file entity that describes the new file. If a file with the same name already exists in the folder, the server will return a 409 Conflict error response.


    #### Update Existing File (file)

    To update an existing file, issue a PUT request to the file's upload link with the raw file data in the request body and the kind query parameter set to "file". The update action will create a new version of the file. The response will contain a WaterButler file entity that describes the updated file.

    #### Rename (files, folders)

    To rename a file or folder, issue a POST request to the move link with the action body parameter set to "rename" and the rename body parameter set to the desired name. The response will contain either a folder entity or file entity with the new name.

    #### Move & Copy (files, folders)

    Move and copy actions both use the same request structure, a POST to the move url, but with different values for the action body parameters. The path parameter is also required and should be the OSF path attribute of the folder being written to. The rename and conflict parameters are optional. If you wish to change the name of the file or folder at its destination, set the rename parameter to the new name. The conflict param governs how name clashes are resolved. Possible values are replace and keep. replace is the default and will overwrite the file that already exists in the target folder. keep will attempt to keep both by adding a suffix to the new file's name until it no longer conflicts. The suffix will be ' (x)' where x is a increasing integer starting from 1. This behavior is intended to mimic that of the OS X Finder. The response will contain either a folder entity or file entity with the new name.
    Files and folders can also be moved between nodes and providers. The resource parameter is the id of the node under which the file/folder should be moved. It must agree with the path parameter, that is the path must identify a valid folder under the node identified by resource. Likewise, the provider parameter may be used to move the file/folder to another storage provider, but both the resource and path parameters must belong to a node and folder already extant on that provider. Both resource and provider default to the current node and providers.
    If a moved/copied file is overwriting an existing file, a 200 OK response will be returned. Otherwise, a 201 Created will be returned.

    #### Delete (file, folders)

    To delete a file or folder send a DELETE request to the delete link. Nothing will be returned in the response body.
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2
  tags: Research, Science, API Provider, Profiles, General Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/file/master/_listings/open-science-framework/filesfile-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/file/master/_listings/open-science-framework/filesfile-id-get-openapi.md
- name: Open Science Framework - Update a file
  x-api-slug: filesfile-id-patch
  description: |-
    Updates the specified file by setting the values of the parameters passed. Any parameters not provided will be left unchanged.
    #### Returns
    Returns JSON with a `data` key containing the new representation of the updated file, if the request is successful.

    If the request is unsuccessful, JSON with an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2
  tags: Research, Science, API Provider, Profiles, General Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/file/master/_listings/open-science-framework/filesfile-id-patch-openapi.md
- name: Open Science Framework - List all file versions
  x-api-slug: filesfile-idversions-get
  description: |-
    A paginated list of all file versions.
    #### Returns
    Returns a JSON object containing `data` and `links` keys.

    The `data` key contains an array of 10 file versions. Each resource in the array is a separate file version object.

    The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).

    If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2
  tags: Research, Science, API Provider, Profiles, General Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/file/master/_listings/open-science-framework/filesfile-idversions-get-openapi.md
- name: Open Science Framework - Retrieve a file version
  x-api-slug: filesfile-idversionsversion-id-get
  description: |-
    Retrieves the details of a file version
    ####Returns

    Returns a JSON object with a `data` key containing the representation of the requested file, if the request was successful.

    If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2
  tags: Research, Science, API Provider, Profiles, General Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/file/master/_listings/open-science-framework/filesfile-idversionsversion-id-get-openapi.md
- name: Open Science Framework - Actions
  x-api-slug: actions-get
  description: |-
    A log can have one of many actions. The complete list of loggable actions (in the format {identifier}: {description}) is as follows:
    * `project_created`: A Node is created
    * `project_registered`: A Node is registered
    * `project_deleted`: A Node is deleted
    * `created_from`: A Node is created using an existing Node as a template
    * `pointer_created`: A Pointer is created
    * `pointer_forked`: A Pointer is forked
    * `pointer_removed`: A Pointer is removed
    * `node_removed`: A component is deleted
    * `node_forked`: A Node is forked
    ---
    * `made_public`: A Node is made public
    * `made_private`: A Node is made private
    * `tag_added`: A tag is added to a Node
    * `tag_removed`: A tag is removed from a Node
    * `edit_title`: A Node's title is changed
    * `edit_description`: A Node's description is changed
    * `updated_fields`: One or more of a Node's fields are changed
    * `external_ids_added`: An external identifier is added to a Node (e.g. DOI, ARK)
    * `view_only_link_added`: A view-only link was added to a Node
    * `view_only_link_removed`:  A view-only link was removed from a Node
    ---
    * `contributor_added`: A Contributor is added to a Node
    * `contributor_removed`: A Contributor is removed from a Node
    * `contributors_reordered`: A Contributor's position in a Node's bibliography is changed
    * `permissions_updated`: A Contributor`s permissions on a Node are changed
    * `made_contributor_visible`: A Contributor is made bibliographically visible on a Node
    * `made_contributor_invisible`: A Contributor is made bibliographically invisible on a Node
    ---
    * `wiki_updated`: A Node's wiki is updated
    * `wiki_deleted`: A Node's wiki is deleted
    * `wiki_renamed`: A Node's wiki is renamed
    * `made_wiki_public`: A Node's wiki is made public
    * `made_wiki_private`: A Node's wiki is made private
    ---
    * `addon_added`: An add-on is linked to a Node
    * `addon_removed`: An add-on is unlinked from a Node
    * `addon_file_moved`: A File in a Node's linked add-on is moved
    * `addon_file_copied`: A File in a Node's linked add-on is copied
    * `addon_file_renamed`: A File in a Node's linked add-on is renamed
    * `node_authorized`: An addon is authorized for a project
    * `node_deauthorized`: An addon is deauthorized for a project
    * `folder_created`: A Folder is created in a Node's linked add-on
    * `file_added`: A File is added to a Node's linked add-on
    * `file_updated`: A File is updated on a Node's linked add-on
    * `file_removed`: A File is removed from a Node's linked add-on
    * `file_restored`: A File is restored in a Node's linked add-on
    ---
    * `comment_added`: A Comment is added to some item
    * `comment_removed`: A Comment is removed from some item
    * `comment_updated`: A Comment is updated on some item
    ---
    * `embargo_initiated`: An embargoed Registration is proposed on a Node
    * `embargo_approved`: A proposed Embargo of a Node is approved
    * `embargo_cancelled`: A proposed Embargo of a Node is cancelled
    * `embargo_completed`: A proposed Embargo of a Node is completed
    * `retraction_initiated`: A Withdrawal of a Registration is proposed
    * `retraction_approved`: A Withdrawal of a Registration is approved
    * `retraction_cancelled`: A Withdrawal of a Registration is cancelled
    * `registration_initiated`: A Registration of a Node is proposed
    * `registration_approved`: A proposed Registration is approved
    * `registration_cancelled`: A proposed Registration is cancelled
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2
  tags: Research, Science, API Provider, Profiles, General Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/file/master/_listings/open-science-framework/actions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/file/master/_listings/open-science-framework/actions-get-openapi.md
- name: Open Science Framework - Actions
  x-api-slug: actions-get
  description: |-
    A log can have one of many actions. The complete list of loggable actions (in the format {identifier}: {description}) is as follows:
    * `project_created`: A Node is created
    * `project_registered`: A Node is registered
    * `project_deleted`: A Node is deleted
    * `created_from`: A Node is created using an existing Node as a template
    * `pointer_created`: A Pointer is created
    * `pointer_forked`: A Pointer is forked
    * `pointer_removed`: A Pointer is removed
    * `node_removed`: A component is deleted
    * `node_forked`: A Node is forked
    ---
    * `made_public`: A Node is made public
    * `made_private`: A Node is made private
    * `tag_added`: A tag is added to a Node
    * `tag_removed`: A tag is removed from a Node
    * `edit_title`: A Node's title is changed
    * `edit_description`: A Node's description is changed
    * `updated_fields`: One or more of a Node's fields are changed
    * `external_ids_added`: An external identifier is added to a Node (e.g. DOI, ARK)
    * `view_only_link_added`: A view-only link was added to a Node
    * `view_only_link_removed`:  A view-only link was removed from a Node
    ---
    * `contributor_added`: A Contributor is added to a Node
    * `contributor_removed`: A Contributor is removed from a Node
    * `contributors_reordered`: A Contributor's position in a Node's bibliography is changed
    * `permissions_updated`: A Contributor`s permissions on a Node are changed
    * `made_contributor_visible`: A Contributor is made bibliographically visible on a Node
    * `made_contributor_invisible`: A Contributor is made bibliographically invisible on a Node
    ---
    * `wiki_updated`: A Node's wiki is updated
    * `wiki_deleted`: A Node's wiki is deleted
    * `wiki_renamed`: A Node's wiki is renamed
    * `made_wiki_public`: A Node's wiki is made public
    * `made_wiki_private`: A Node's wiki is made private
    ---
    * `addon_added`: An add-on is linked to a Node
    * `addon_removed`: An add-on is unlinked from a Node
    * `addon_file_moved`: A File in a Node's linked add-on is moved
    * `addon_file_copied`: A File in a Node's linked add-on is copied
    * `addon_file_renamed`: A File in a Node's linked add-on is renamed
    * `node_authorized`: An addon is authorized for a project
    * `node_deauthorized`: An addon is deauthorized for a project
    * `folder_created`: A Folder is created in a Node's linked add-on
    * `file_added`: A File is added to a Node's linked add-on
    * `file_updated`: A File is updated on a Node's linked add-on
    * `file_removed`: A File is removed from a Node's linked add-on
    * `file_restored`: A File is restored in a Node's linked add-on
    ---
    * `comment_added`: A Comment is added to some item
    * `comment_removed`: A Comment is removed from some item
    * `comment_updated`: A Comment is updated on some item
    ---
    * `embargo_initiated`: An embargoed Registration is proposed on a Node
    * `embargo_approved`: A proposed Embargo of a Node is approved
    * `embargo_cancelled`: A proposed Embargo of a Node is cancelled
    * `embargo_completed`: A proposed Embargo of a Node is completed
    * `retraction_initiated`: A Withdrawal of a Registration is proposed
    * `retraction_approved`: A Withdrawal of a Registration is approved
    * `retraction_cancelled`: A Withdrawal of a Registration is cancelled
    * `registration_initiated`: A Registration of a Node is proposed
    * `registration_approved`: A proposed Registration is approved
    * `registration_cancelled`: A proposed Registration is cancelled
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2
  tags: Research, Science, API Provider, Profiles, General Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/file/master/_listings/open-science-framework/actions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/file/master/_listings/open-science-framework/actions-get-openapi.md
x-common:
- type: x-website
  url: https://cos.io
- type: x-api-gallery
  url: http://open.fintech.api.gallery.streamdata.io
- type: x-api-stack
  url: http://open.science.framework.stack.network
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