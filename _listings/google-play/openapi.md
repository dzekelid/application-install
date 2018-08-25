---
swagger: "2.0"
x-collection-name: Google Play
x-complete: 1
info:
  title: Google Play
  version: 1.0.0
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
    put:
      summary: Update App Install
      description: Requests to install the latest version of an app to a device. If
        the app is already installed, then it is updated to the latest version if
        necessary.
      operationId: androidenterprise.installs.update
      x-api-path-slug: enterprisesenterpriseidusersuseriddevicesdeviceidinstallsinstallid-put
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
  /enterprises/{enterpriseId}/users/{userId}/devices/{deviceId}/managedConfigurationsForDevice:
    get:
      summary: Get Per Device App Installs
      description: Lists all the per-device managed configurations for the specified
        device. Only the ID is set.
      operationId: androidenterprise.managedconfigurationsfordevice.list
      x-api-path-slug: enterprisesenterpriseidusersuseriddevicesdeviceidmanagedconfigurationsfordevice-get
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
  /enterprises/{enterpriseId}/users/{userId}/devices/{deviceId}/managedConfigurationsForDevice/{managedConfigurationForDeviceId}:
    delete:
      summary: Remove Per Device App Install
      description: Removes a per-device managed configuration for an app for the specified
        device.
      operationId: androidenterprise.managedconfigurationsfordevice.delete
      x-api-path-slug: enterprisesenterpriseidusersuseriddevicesdeviceidmanagedconfigurationsfordevicemanagedconfigurationfordeviceid-delete
      parameters:
      - in: path
        name: deviceId
        description: The Android ID of the device
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      - in: path
        name: managedConfigurationForDeviceId
        description: The ID of the managed configuration (a product ID), e
      - in: path
        name: userId
        description: The ID of the user
      responses:
        200:
          description: OK
      tags:
      - App Install
    get:
      summary: Get Per Device App Install
      description: Retrieves details of a per-device managed configuration.
      operationId: androidenterprise.managedconfigurationsfordevice.get
      x-api-path-slug: enterprisesenterpriseidusersuseriddevicesdeviceidmanagedconfigurationsfordevicemanagedconfigurationfordeviceid-get
      parameters:
      - in: path
        name: deviceId
        description: The Android ID of the device
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      - in: path
        name: managedConfigurationForDeviceId
        description: The ID of the managed configuration (a product ID), e
      - in: path
        name: userId
        description: The ID of the user
      responses:
        200:
          description: OK
      tags:
      - App Install
    patch:
      summary: Update Per Device App Install
      description: Adds or updates a per-device managed configuration for an app for
        the specified device. This method supports patch semantics.
      operationId: androidenterprise.managedconfigurationsfordevice.patch
      x-api-path-slug: enterprisesenterpriseidusersuseriddevicesdeviceidmanagedconfigurationsfordevicemanagedconfigurationfordeviceid-patch
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
        name: managedConfigurationForDeviceId
        description: The ID of the managed configuration (a product ID), e
      - in: path
        name: userId
        description: The ID of the user
      responses:
        200:
          description: OK
      tags:
      - App Install
    put:
      summary: Update Per Device App Install
      description: Adds or updates a per-device managed configuration for an app for
        the specified device.
      operationId: androidenterprise.managedconfigurationsfordevice.update
      x-api-path-slug: enterprisesenterpriseidusersuseriddevicesdeviceidmanagedconfigurationsfordevicemanagedconfigurationfordeviceid-put
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
        name: managedConfigurationForDeviceId
        description: The ID of the managed configuration (a product ID), e
      - in: path
        name: userId
        description: The ID of the user
      responses:
        200:
          description: OK
      tags:
      - App Install
  /enterprises/{enterpriseId}/users/{userId}/devices/{deviceId}/state:
    get:
      summary: Get Per Device App Install State
      description: Retrieves whether a device's access to Google services is enabled
        or disabled. The device state takes effect only if enforcing EMM policies
        on Android devices is enabled in the Google Admin Console. Otherwise, the
        device state is ignored and all devices are allowed access to Google services.
        This is only supported for Google-managed users.
      operationId: androidenterprise.devices.getState
      x-api-path-slug: enterprisesenterpriseidusersuseriddevicesdeviceidstate-get
      parameters:
      - in: path
        name: deviceId
        description: The ID of the device
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
    put:
      summary: Update Per Device App Install State
      description: Sets whether a device's access to Google services is enabled or
        disabled. The device state takes effect only if enforcing EMM policies on
        Android devices is enabled in the Google Admin Console. Otherwise, the device
        state is ignored and all devices are allowed access to Google services. This
        is only supported for Google-managed users.
      operationId: androidenterprise.devices.setState
      x-api-path-slug: enterprisesenterpriseidusersuseriddevicesdeviceidstate-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: deviceId
        description: The ID of the device
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
---