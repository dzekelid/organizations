---
swagger: "2.0"
x-collection-name: Trello
x-complete: 0
info:
  title: Trello Put Organizations
  description: Put organizations.
  termsOfService: https://trello.com/legal
  contact:
    name: Trello
    url: https://trello.com/home
  version: "1.0"
host: trello.com
basePath: /1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /members/{idMember}/organizations:
    get:
      summary: Get Members Organizations
      description: Get members organizations.
      operationId: getMembersOrganizationsByIdMember
      x-api-path-slug: membersidmemberorganizations-get
      parameters:
      - in: query
        name: fields
        description: 'all or a comma-separated list of: billableMemberCount, desc,
          descData, displayName, idBoards, invitations, invited, logoHash, memberships,
          name, powerUps, prefs, premiumFeatures, products, url or website'
      - in: query
        name: filter
        description: 'One of: all, members, none or public'
      - in: path
        name: idMember
        description: idMember or username
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: paid_account
        description: true or false
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Members
      - Organizations
  /members/{idMember}/organizations/{filter}:
    get:
      summary: Get Members Organizations Filter
      description: Get members organizations filter.
      operationId: getMembersOrganizationsByIdMemberByFilter
      x-api-path-slug: membersidmemberorganizationsfilter-get
      parameters:
      - in: path
        name: filter
        description: filter
      - in: path
        name: idMember
        description: idMember or username
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Members
      - Organizations
      - Filter
  /organizations:
    post:
      summary: Post Organizations
      description: Post organizations.
      operationId: addOrganizations
      x-api-path-slug: organizations-post
      parameters:
      - in: body
        name: body
        description: Attributes of Organizations to be added
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Organizations
  /organizations/{idOrg}:
    delete:
      summary: Delete Organizations
      description: Delete organizations.
      operationId: deleteOrganizationsByIdOrg
      x-api-path-slug: organizationsidorg-delete
      parameters:
      - in: path
        name: idOrg
        description: idOrg or name
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Organizations
    get:
      summary: Get Organizations
      description: Get organizations.
      operationId: getOrganizationsByIdOrg
      x-api-path-slug: organizationsidorg-get
      parameters:
      - in: query
        name: actions
        description: 'all or a comma-separated list of: addAttachmentToCard, addChecklistToCard,
          addMemberToBoard, addMemberToCard, addMemberToOrganization, addToOrganizationBoard,
          commentCard, convertToCardFromCheckItem, copyBoard, copyCard, copyCommentCard,
          createBoard, createCard, createList, createOrganization, deleteAttachmentFromCard,
          deleteBoardInvitation, deleteCard, deleteOrganizationInvitation, disablePowerUp,
          emailCard, enablePowerUp, makeAdminOfBoard, makeNormalMemberOfBoard, makeNormalMemberOfOrganization,
          makeObserverOfBoard, memberJoinedTrello, moveCardFromBoard, moveCardToBoard,
          moveListFromBoard, moveListToBoard, removeChecklistFromCard, removeFromOrganizationBoard,
          removeMemberFromCard, unconfirmedBoardInvitation, unconfirmedOrganizationInvitation,
          updateBoard, updateCard, updateCard:closed, updateCard:desc, updateCard:idList,
          updateCard:name, updateCheckItemStateOnCard, updateChecklist, updateList,
          updateList:closed, updateList:name, updateMember or updateOrganization'
      - in: query
        name: actions_display
        description: true or false
      - in: query
        name: actions_entities
        description: true or false
      - in: query
        name: actions_limit
        description: a number from 0 to 1000
      - in: query
        name: action_fields
        description: 'all or a comma-separated list of: data, date, idMemberCreator
          or type'
      - in: query
        name: boards
        description: 'all or a comma-separated list of: closed, members, open, organization,
          pinned, public, starred or unpinned'
      - in: query
        name: board_actions
        description: 'all or a comma-separated list of: addAttachmentToCard, addChecklistToCard,
          addMemberToBoard, addMemberToCard, addMemberToOrganization, addToOrganizationBoard,
          commentCard, convertToCardFromCheckItem, copyBoard, copyCard, copyCommentCard,
          createBoard, createCard, createList, createOrganization, deleteAttachmentFromCard,
          deleteBoardInvitation, deleteCard, deleteOrganizationInvitation, disablePowerUp,
          emailCard, enablePowerUp, makeAdminOfBoard, makeNormalMemberOfBoard, makeNormalMemberOfOrganization,
          makeObserverOfBoard, memberJoinedTrello, moveCardFromBoard, moveCardToBoard,
          moveListFromBoard, moveListToBoard, removeChecklistFromCard, removeFromOrganizationBoard,
          removeMemberFromCard, unconfirmedBoardInvitation, unconfirmedOrganizationInvitation,
          updateBoard, updateCard, updateCard:closed, updateCard:desc, updateCard:idList,
          updateCard:name, updateCheckItemStateOnCard, updateChecklist, updateList,
          updateList:closed, updateList:name, updateMember or updateOrganization'
      - in: query
        name: board_actions_display
        description: true or false
      - in: query
        name: board_actions_entities
        description: true or false
      - in: query
        name: board_actions_format
        description: 'One of: count, list or minimal'
      - in: query
        name: board_actions_limit
        description: a number from 0 to 1000
      - in: query
        name: board_actions_since
        description: A date, null or lastView
      - in: query
        name: board_action_fields
        description: 'all or a comma-separated list of: data, date, idMemberCreator
          or type'
      - in: query
        name: board_fields
        description: 'all or a comma-separated list of: closed, dateLastActivity,
          dateLastView, desc, descData, idOrganization, invitations, invited, labelNames,
          memberships, name, pinned, powerUps, prefs, shortLink, shortUrl, starred,
          subscribed or url'
      - in: query
        name: board_lists
        description: 'One of: all, closed, none or open'
      - in: query
        name: fields
        description: 'all or a comma-separated list of: billableMemberCount, desc,
          descData, displayName, idBoards, invitations, invited, logoHash, memberships,
          name, powerUps, prefs, premiumFeatures, products, url or website'
      - in: path
        name: idOrg
        description: idOrg or name
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: members
        description: 'One of: admins, all, none, normal or owners'
      - in: query
        name: memberships
        description: 'all or a comma-separated list of: active, admin, deactivated,
          me or normal'
      - in: query
        name: memberships_member
        description: true or false
      - in: query
        name: memberships_member_fields
        description: 'all or a comma-separated list of: avatarHash, bio, bioData,
          confirmed, fullName, idPremOrgsAdmin, initials, memberType, products, status,
          url or username'
      - in: query
        name: membersInvited
        description: 'One of: admins, all, none, normal or owners'
      - in: query
        name: membersInvited_fields
        description: 'all or a comma-separated list of: avatarHash, bio, bioData,
          confirmed, fullName, idPremOrgsAdmin, initials, memberType, products, status,
          url or username'
      - in: query
        name: member_activity
        description: true or false ; works for premium organizations only
      - in: query
        name: member_fields
        description: 'all or a comma-separated list of: avatarHash, bio, bioData,
          confirmed, fullName, idPremOrgsAdmin, initials, memberType, products, status,
          url or username'
      - in: query
        name: paid_account
        description: true or false
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Organizations
    put:
      summary: Put Organizations
      description: Put organizations.
      operationId: updateOrganizationsByIdOrg
      x-api-path-slug: organizationsidorg-put
      parameters:
      - in: body
        name: body
        description: Attributes of Organizations to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idOrg
        description: idOrg or name
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Organizations
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