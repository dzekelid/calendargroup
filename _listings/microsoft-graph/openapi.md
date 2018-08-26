---
swagger: "2.0"
x-collection-name: Microsoft Graph
x-complete: 1
info:
  title: Microsoft Graph API
  description: microsoft-graph-exposes-multiple-apis-from-office-365-and-other-microsoft-cloud-services-through-a-single-endpoint-httpsgraph-microsoft-com--microsoft-graph-simplifies-queries-that-would-otherwise-be-more-complex-
  version: 1.0.0
host: graph.microsoft.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /me/calendarGroups/{id}:
    patch:
      summary: Update Calendargroup
      description: Update calendargroup Update the properties of calendargroup object.
      operationId: UpdateCalendargroup
      x-api-path-slug: mecalendargroupsid-patch
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: header
        name: Content-Type
        description: application/json
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Calendargroup
  /users/{id | userPrincipalName}/calendarGroups/{id}:
    patch:
      summary: Update Calendargroup
      description: Update calendargroup Update the properties of calendargroup object.
      operationId: UpdateCalendargroup
      x-api-path-slug: usersid--userprincipalnamecalendargroupsid-patch
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: header
        name: Content-Type
        description: application/json
      - in: path
        name: id
        type: string
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - Calendargroup
---