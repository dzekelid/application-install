---
name: Google Play
x-slug: google-play
description: 'The Google Play Developer API allows you to perform a number of publishing
  and app-management tasks. It includes two components: The Subscriptions and In-App
  Purchases API lets you manage in-app purchases and subscriptions. The Publishing
  API lets you upload and publish apps, and perform other publishing-related tasks.'
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-play.png
x-kinRank: "9"
x-alexaRank: "0"
tags: Application Install
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/application-install/master/_listings/google-play/apis.md
specificationVersion: "0.14"
apis:
- name: Google Play - Get App Installs
  x-api-slug: enterprisesenterpriseidusersuseriddevicesdeviceidinstalls-get
  description: Retrieves the details of all apps installed on the specified device.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-play.png
  humanURL: https://play.google.com/store
  baseURL: https:///
  tags: Google APIs, Android, Mobile, Gaming, Games, Movies, Stack Network, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/application-install/master/_listings/google-play/enterprisesenterpriseidusersuseriddevicesdeviceidinstalls-get-openapi.md
- name: Google Play - Remove App Install
  x-api-slug: enterprisesenterpriseidusersuseriddevicesdeviceidinstallsinstallid-delete
  description: Requests to remove an app from a device. A call to get or list will
    still show the app as installed on the device until it is actually removed.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-play.png
  humanURL: https://play.google.com/store
  baseURL: https:///
  tags: Google APIs, Android, Mobile, Gaming, Games, Movies, Stack Network, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/application-install/master/_listings/google-play/enterprisesenterpriseidusersuseriddevicesdeviceidinstallsinstallid-delete-openapi.md
- name: Google Play - Get App Install
  x-api-slug: enterprisesenterpriseidusersuseriddevicesdeviceidinstallsinstallid-get
  description: Retrieves details of an installation of an app on a device.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-play.png
  humanURL: https://play.google.com/store
  baseURL: https:///
  tags: Google APIs, Android, Mobile, Gaming, Games, Movies, Stack Network, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/application-install/master/_listings/google-play/enterprisesenterpriseidusersuseriddevicesdeviceidinstallsinstallid-get-openapi.md
- name: Google Play - Update App Install
  x-api-slug: enterprisesenterpriseidusersuseriddevicesdeviceidinstallsinstallid-patch
  description: Requests to install the latest version of an app to a device. If the
    app is already installed, then it is updated to the latest version if necessary.
    This method supports patch semantics.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-play.png
  humanURL: https://play.google.com/store
  baseURL: https:///
  tags: Google APIs, Android, Mobile, Gaming, Games, Movies, Stack Network, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/application-install/master/_listings/google-play/enterprisesenterpriseidusersuseriddevicesdeviceidinstallsinstallid-patch-openapi.md
- name: Google Play - Update App Install
  x-api-slug: enterprisesenterpriseidusersuseriddevicesdeviceidinstallsinstallid-put
  description: Requests to install the latest version of an app to a device. If the
    app is already installed, then it is updated to the latest version if necessary.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-play.png
  humanURL: https://play.google.com/store
  baseURL: https:///
  tags: Google APIs, Android, Mobile, Gaming, Games, Movies, Stack Network, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/application-install/master/_listings/google-play/enterprisesenterpriseidusersuseriddevicesdeviceidinstallsinstallid-put-openapi.md
- name: Google Play - Get Per Device App Installs
  x-api-slug: enterprisesenterpriseidusersuseriddevicesdeviceidmanagedconfigurationsfordevice-get
  description: Lists all the per-device managed configurations for the specified device.
    Only the ID is set.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-play.png
  humanURL: https://play.google.com/store
  baseURL: https:///
  tags: Google APIs, Android, Mobile, Gaming, Games, Movies, Stack Network, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/application-install/master/_listings/google-play/enterprisesenterpriseidusersuseriddevicesdeviceidmanagedconfigurationsfordevice-get-openapi.md
- name: Google Play - Remove Per Device App Install
  x-api-slug: enterprisesenterpriseidusersuseriddevicesdeviceidmanagedconfigurationsfordevicemanagedconfigurationfordeviceid-delete
  description: Removes a per-device managed configuration for an app for the specified
    device.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-play.png
  humanURL: https://play.google.com/store
  baseURL: https:///
  tags: Google APIs, Android, Mobile, Gaming, Games, Movies, Stack Network, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/application-install/master/_listings/google-play/enterprisesenterpriseidusersuseriddevicesdeviceidmanagedconfigurationsfordevicemanagedconfigurationfordeviceid-delete-openapi.md
- name: Google Play - Get Per Device App Install
  x-api-slug: enterprisesenterpriseidusersuseriddevicesdeviceidmanagedconfigurationsfordevicemanagedconfigurationfordeviceid-get
  description: Retrieves details of a per-device managed configuration.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-play.png
  humanURL: https://play.google.com/store
  baseURL: https:///
  tags: Google APIs, Android, Mobile, Gaming, Games, Movies, Stack Network, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/application-install/master/_listings/google-play/enterprisesenterpriseidusersuseriddevicesdeviceidmanagedconfigurationsfordevicemanagedconfigurationfordeviceid-get-openapi.md
- name: Google Play - Update Per Device App Install
  x-api-slug: enterprisesenterpriseidusersuseriddevicesdeviceidmanagedconfigurationsfordevicemanagedconfigurationfordeviceid-patch
  description: Adds or updates a per-device managed configuration for an app for the
    specified device. This method supports patch semantics.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-play.png
  humanURL: https://play.google.com/store
  baseURL: https:///
  tags: Google APIs, Android, Mobile, Gaming, Games, Movies, Stack Network, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/application-install/master/_listings/google-play/enterprisesenterpriseidusersuseriddevicesdeviceidmanagedconfigurationsfordevicemanagedconfigurationfordeviceid-patch-openapi.md
- name: Google Play - Update Per Device App Install
  x-api-slug: enterprisesenterpriseidusersuseriddevicesdeviceidmanagedconfigurationsfordevicemanagedconfigurationfordeviceid-put
  description: Adds or updates a per-device managed configuration for an app for the
    specified device.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-play.png
  humanURL: https://play.google.com/store
  baseURL: https:///
  tags: Google APIs, Android, Mobile, Gaming, Games, Movies, Stack Network, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/application-install/master/_listings/google-play/enterprisesenterpriseidusersuseriddevicesdeviceidmanagedconfigurationsfordevicemanagedconfigurationfordeviceid-put-openapi.md
- name: Google Play - Get Per Device App Install State
  x-api-slug: enterprisesenterpriseidusersuseriddevicesdeviceidstate-get
  description: Retrieves whether a device's access to Google services is enabled or
    disabled. The device state takes effect only if enforcing EMM policies on Android
    devices is enabled in the Google Admin Console. Otherwise, the device state is
    ignored and all devices are allowed access to Google services. This is only supported
    for Google-managed users.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-play.png
  humanURL: https://play.google.com/store
  baseURL: https:///
  tags: Google APIs, Android, Mobile, Gaming, Games, Movies, Stack Network, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/application-install/master/_listings/google-play/enterprisesenterpriseidusersuseriddevicesdeviceidstate-get-openapi.md
- name: Google Play - Update Per Device App Install State
  x-api-slug: enterprisesenterpriseidusersuseriddevicesdeviceidstate-put
  description: Sets whether a device's access to Google services is enabled or disabled.
    The device state takes effect only if enforcing EMM policies on Android devices
    is enabled in the Google Admin Console. Otherwise, the device state is ignored
    and all devices are allowed access to Google services. This is only supported
    for Google-managed users.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-play.png
  humanURL: https://play.google.com/store
  baseURL: https:///
  tags: Google APIs, Android, Mobile, Gaming, Games, Movies, Stack Network, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/application-install/master/_listings/google-play/enterprisesenterpriseidusersuseriddevicesdeviceidstate-put-openapi.md
x-common:
- type: x-api-gallery
  url: http://google.people.api.gallery.streamdata.io
- type: x-api-stack
  url: http://google.play.stack.network
- type: x-blog
  url: https://blog.google/products/google-play/
- type: x-blog-rss
  url: https://blog.google/products/google-play/rss
- type: x-developer
  url: https://developers.google.com/android-publisher/
- type: x-facebook
  url: https://www.facebook.com/GooglePlay
- type: x-getting-started
  url: https://developers.google.com/android-publisher/getting_started
- type: x-twitter
  url: https://twitter.com/GooglePlay
- type: x-website
  url: https://play.google.com/store
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---