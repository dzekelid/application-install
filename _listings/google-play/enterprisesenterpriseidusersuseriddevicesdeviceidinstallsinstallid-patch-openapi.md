---
swagger: "2.0"
x-collection-name: Google Play
x-complete: 0
info:
  title: Google Play Update App Install
  version: 1.0.0
  description: Requests to install the latest version of an app to a device. If the
    app is already installed, then it is updated to the latest version if necessary.
    This method supports patch semantics.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /enterprises/{enterpriseId}/users/{userId}/devices/{deviceId}/installs:
    get:
      summary: Get App Installs
      description: Retrieves the details of all apps installed on the specified device.
      operationId: androidenterprise.installs.list
      x-api-path-slug: enterprisesenterpriseidusersuseriddevicesdeviceidinstalls-get
      parameters:
      - in: path
        name: deviceId
        description: The Android ID of the device
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      - in: path
        name: userId
        description: The ID of the user
      responses:
        200:
          description: OK
      tags:
      - App Install
  /enterprises/{enterpriseId}/users/{userId}/devices/{deviceId}/installs/{installId}:
    delete:
      summary: Remove App Install
      description: Requests to remove an app from a device. A call to get or list
        will still show the app as installed on the device until it is actually removed.
      operationId: androidenterprise.installs.delete
      x-api-path-slug: enterprisesenterpriseidusersuseriddevicesdeviceidinstallsinstallid-delete
      parameters:
      - in: path
        name: deviceId
        description: The Android ID of the device
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      - in: path
        name: installId
        description: The ID of the product represented by the install, e
      - in: path
        name: userId
        description: The ID of the user
      responses:
        200:
          description: OK
      tags:
      - App Install
    get:
      summary: Get App Install
      description: Retrieves details of an installation of an app on a device.
      operationId: androidenterprise.installs.get
      x-api-path-slug: enterprisesenterpriseidusersuseriddevicesdeviceidinstallsinstallid-get
      parameters:
      - in: path
        name: deviceId
        description: The Android ID of the device
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      - in: path
        name: installId
        description: The ID of the product represented by the install, e
      - in: path
        name: userId
        description: The ID of the user
      responses:
        200:
          description: OK
      tags:
      - App Install
    patch:
      summary: Update App Install
      description: Requests to install the latest version of an app to a device. If
        the app is already installed, then it is updated to the latest version if
        necessary. This method supports patch semantics.
      operationId: androidenterprise.installs.patch
      x-api-path-slug: enterprisesenterpriseidusersuseriddevicesdeviceidinstallsinstallid-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: deviceId
        description: The Android ID of the device
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      - in: path
        name: installId
        description: The ID of the product represented by the install, e
      - in: path
        name: userId
        description: The ID of the user
      responses:
        200:
          description: OK
      tags:
      - App Install
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