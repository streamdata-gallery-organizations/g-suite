---
swagger: "2.0"
info:
  title: G Suite Activity
  description: Provides a historical view of activity.
  contact:
    name: Google
    url: https://google.com
  version: v1
host: www.googleapis.com
basePath: /appsactivity/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /activities:
    get:
      summary: Get Activity
      description: Returns a list of activities visible to the current logged in user
      operationId: appsactivity.activities.list
      parameters:
      - in: query
        name: drive.ancestorId
        description: Identifies the Drive folder containing the items for which to
          return activities
      - in: query
        name: drive.fileId
        description: Identifies the Drive item to return activities for
      - in: query
        name: groupingStrategy
        description: Indicates the strategy to use when grouping singleEvents items
          in the associated combinedEvent object
      - in: query
        name: pageSize
        description: The maximum number of events to return on a page
      - in: query
        name: pageToken
        description: A token to retrieve a specific page of results
      - in: query
        name: source
        description: The Google service from which to return activities
      - in: query
        name: userId
        description: Indicates the user to return activity for
      responses:
        200:
          description: OK
      tags:
      - activities
definitions:
  Activity:
    properties:
      singleEvents:
        description: This is a default description.
        type: parameters
  Event:
    properties:
      additionalEventTypes:
        description: This is a default description.
        type: parameters
      eventTimeMillis:
        description: This is a default description.
        type: parameters
      fromUserDeletion:
        description: This is a default description.
        type: parameters
      permissionChanges:
        description: This is a default description.
        type: parameters
      primaryEventType:
        description: This is a default description.
        type: parameters
  ListActivitiesResponse:
    properties:
      activities:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
  Move:
    properties:
      addedParents:
        description: This is a default description.
        type: parameters
      removedParents:
        description: This is a default description.
        type: parameters
  Parent:
    properties:
      id:
        description: This is a default description.
        type: parameters
      isRoot:
        description: This is a default description.
        type: parameters
      title:
        description: This is a default description.
        type: parameters
  Permission:
    properties:
      name:
        description: This is a default description.
        type: parameters
      permissionId:
        description: This is a default description.
        type: parameters
      role:
        description: This is a default description.
        type: parameters
      type:
        description: This is a default description.
        type: parameters
      withLink:
        description: This is a default description.
        type: parameters
  PermissionChange:
    properties:
      addedPermissions:
        description: This is a default description.
        type: parameters
      removedPermissions:
        description: This is a default description.
        type: parameters
  Photo:
    properties:
      url:
        description: This is a default description.
        type: parameters
  Rename:
    properties:
      newTitle:
        description: This is a default description.
        type: parameters
      oldTitle:
        description: This is a default description.
        type: parameters
  Target:
    properties:
      id:
        description: This is a default description.
        type: parameters
      mimeType:
        description: This is a default description.
        type: parameters
      name:
        description: This is a default description.
        type: parameters
  User:
    properties:
      isDeleted:
        description: This is a default description.
        type: parameters
      isMe:
        description: This is a default description.
        type: parameters
      name:
        description: This is a default description.
        type: parameters
      permissionId:
        description: This is a default description.
        type: parameters
x-collection-name: G Suite
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