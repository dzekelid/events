---
name: Kubernetes
x-slug: kubernetes
description: Manage a cluster of Linux containers as a single system to accelerate
  Dev and simplify Ops. Kubernetes is an open source orchestration system for Docker
  containers. It handles scheduling onto nodes in a compute cluster and actively manages
  workloads to ensure that their state matches the users declared intentions. Using
  the concepts of labels and pods, it groups the containers which make up an application
  into logical units for easy management and discovery.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/kubernetes-logo.png
x-kinRank: "8"
x-alexaRank: "0"
tags: Events
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/kubernetes/apis.md
specificationVersion: "0.14"
apis:
- name: Kubernetes - Get Events
  x-api-slug: apiv1beta3events-get
  description: List objects of kind event.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/kubernetes-logo.png
  humanURL: http://kubernetes.io/
  baseURL: :///api/v1beta3/127.0.0.1:6443
  tags: Containers, Google, Stack Network, API Service Provider, Containers, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/kubernetes/apiv1beta3events-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/kubernetes/apiv1beta3events-get-openapi.md
- name: Kubernetes - Get Namespaces Events
  x-api-slug: apiv1beta3namespacesnamespacesevents-get
  description: List objects of kind event.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/kubernetes-logo.png
  humanURL: http://kubernetes.io/
  baseURL: :///api/v1beta3/127.0.0.1:6443
  tags: Containers, Google, Stack Network, API Service Provider, Containers, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/kubernetes/apiv1beta3namespacesnamespacesevents-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/kubernetes/apiv1beta3namespacesnamespacesevents-get-openapi.md
- name: Kubernetes - Post Namespaces Events
  x-api-slug: apiv1beta3namespacesnamespacesevents-post
  description: Create a event.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/kubernetes-logo.png
  humanURL: http://kubernetes.io/
  baseURL: :///api/v1beta3/127.0.0.1:6443
  tags: Containers, Google, Stack Network, API Service Provider, Containers, Profiles,
    Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/kubernetes/apiv1beta3namespacesnamespacesevents-post-openapi.md
- name: Kubernetes - Delete Namespaces Events Name
  x-api-slug: apiv1beta3namespacesnamespaceseventsname-delete
  description: Delete a event.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/kubernetes-logo.png
  humanURL: http://kubernetes.io/
  baseURL: :///api/v1beta3/127.0.0.1:6443
  tags: Containers, Google, Stack Network, API Service Provider, Containers, Profiles,
    Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/kubernetes/apiv1beta3namespacesnamespaceseventsname-delete-openapi.md
- name: Kubernetes - Get Namespaces Events Name
  x-api-slug: apiv1beta3namespacesnamespaceseventsname-get
  description: Read the specified event.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/kubernetes-logo.png
  humanURL: http://kubernetes.io/
  baseURL: :///api/v1beta3/127.0.0.1:6443
  tags: Containers, Google, Stack Network, API Service Provider, Containers, Profiles,
    Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/kubernetes/apiv1beta3namespacesnamespaceseventsname-get-openapi.md
- name: Kubernetes - Put Namespaces Events Name
  x-api-slug: apiv1beta3namespacesnamespaceseventsname-put
  description: Update the specified event.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/kubernetes-logo.png
  humanURL: http://kubernetes.io/
  baseURL: :///api/v1beta3/127.0.0.1:6443
  tags: Containers, Google, Stack Network, API Service Provider, Containers, Profiles,
    Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/kubernetes/apiv1beta3namespacesnamespaceseventsname-put-openapi.md
- name: Kubernetes - Get Watch Events
  x-api-slug: apiv1beta3watchevents-get
  description: Watch a list of event.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/kubernetes-logo.png
  humanURL: http://kubernetes.io/
  baseURL: :///api/v1beta3/127.0.0.1:6443
  tags: Containers, Google, Stack Network, API Service Provider, Containers, Profiles,
    Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/kubernetes/apiv1beta3watchevents-get-openapi.md
- name: Kubernetes - Get Watch Namespaces Events
  x-api-slug: apiv1beta3watchnamespacesnamespacesevents-get
  description: Watch a list of event.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/kubernetes-logo.png
  humanURL: http://kubernetes.io/
  baseURL: :///api/v1beta3/127.0.0.1:6443
  tags: Containers, Google, Stack Network, API Service Provider, Containers, Profiles,
    Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/kubernetes/apiv1beta3watchnamespacesnamespacesevents-get-openapi.md
- name: Kubernetes - Get Watch Namespaces Events Name
  x-api-slug: apiv1beta3watchnamespacesnamespaceseventsname-get
  description: Watch a particular event.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/kubernetes-logo.png
  humanURL: http://kubernetes.io/
  baseURL: :///api/v1beta3/127.0.0.1:6443
  tags: Containers, Google, Stack Network, API Service Provider, Containers, Profiles,
    Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/kubernetes/apiv1beta3watchnamespacesnamespaceseventsname-get-openapi.md
- name: Kubernetes - Get Events
  x-api-slug: apiv1beta3events-get
  description: List objects of kind event.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/kubernetes-logo.png
  humanURL: http://kubernetes.io/
  baseURL: :///api/v1beta3/127.0.0.1:6443
  tags: Containers, Google, Stack Network, API Service Provider, Containers, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/kubernetes/apiv1beta3events-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/kubernetes/apiv1beta3events-get-openapi.md
- name: Kubernetes - Get Namespaces Events
  x-api-slug: apiv1beta3namespacesnamespacesevents-get
  description: List objects of kind event.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/kubernetes-logo.png
  humanURL: http://kubernetes.io/
  baseURL: :///api/v1beta3/127.0.0.1:6443
  tags: Containers, Google, Stack Network, API Service Provider, Containers, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/kubernetes/apiv1beta3namespacesnamespacesevents-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/kubernetes/apiv1beta3namespacesnamespacesevents-get-openapi.md
- name: Kubernetes - Post Namespaces Events
  x-api-slug: apiv1beta3namespacesnamespacesevents-post
  description: Create a event.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/kubernetes-logo.png
  humanURL: http://kubernetes.io/
  baseURL: :///api/v1beta3/127.0.0.1:6443
  tags: Containers, Google, Stack Network, API Service Provider, Containers, Profiles,
    Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/kubernetes/apiv1beta3namespacesnamespacesevents-post-openapi.md
- name: Kubernetes - Delete Namespaces Events Name
  x-api-slug: apiv1beta3namespacesnamespaceseventsname-delete
  description: Delete a event.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/kubernetes-logo.png
  humanURL: http://kubernetes.io/
  baseURL: :///api/v1beta3/127.0.0.1:6443
  tags: Containers, Google, Stack Network, API Service Provider, Containers, Profiles,
    Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/kubernetes/apiv1beta3namespacesnamespaceseventsname-delete-openapi.md
- name: Kubernetes - Get Namespaces Events Name
  x-api-slug: apiv1beta3namespacesnamespaceseventsname-get
  description: Read the specified event.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/kubernetes-logo.png
  humanURL: http://kubernetes.io/
  baseURL: :///api/v1beta3/127.0.0.1:6443
  tags: Containers, Google, Stack Network, API Service Provider, Containers, Profiles,
    Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/kubernetes/apiv1beta3namespacesnamespaceseventsname-get-openapi.md
- name: Kubernetes - Put Namespaces Events Name
  x-api-slug: apiv1beta3namespacesnamespaceseventsname-put
  description: Update the specified event.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/kubernetes-logo.png
  humanURL: http://kubernetes.io/
  baseURL: :///api/v1beta3/127.0.0.1:6443
  tags: Containers, Google, Stack Network, API Service Provider, Containers, Profiles,
    Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/kubernetes/apiv1beta3namespacesnamespaceseventsname-put-openapi.md
- name: Kubernetes - Get Watch Events
  x-api-slug: apiv1beta3watchevents-get
  description: Watch a list of event.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/kubernetes-logo.png
  humanURL: http://kubernetes.io/
  baseURL: :///api/v1beta3/127.0.0.1:6443
  tags: Containers, Google, Stack Network, API Service Provider, Containers, Profiles,
    Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/kubernetes/apiv1beta3watchevents-get-openapi.md
- name: Kubernetes - Get Watch Namespaces Events
  x-api-slug: apiv1beta3watchnamespacesnamespacesevents-get
  description: Watch a list of event.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/kubernetes-logo.png
  humanURL: http://kubernetes.io/
  baseURL: :///api/v1beta3/127.0.0.1:6443
  tags: Containers, Google, Stack Network, API Service Provider, Containers, Profiles,
    Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/kubernetes/apiv1beta3watchnamespacesnamespacesevents-get-openapi.md
- name: Kubernetes - Get Watch Namespaces Events Name
  x-api-slug: apiv1beta3watchnamespacesnamespaceseventsname-get
  description: Watch a particular event.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/kubernetes-logo.png
  humanURL: http://kubernetes.io/
  baseURL: :///api/v1beta3/127.0.0.1:6443
  tags: Containers, Google, Stack Network, API Service Provider, Containers, Profiles,
    Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/kubernetes/apiv1beta3watchnamespacesnamespaceseventsname-get-openapi.md
- name: Kubernetes - Get Events
  x-api-slug: apiv1beta3events-get
  description: List objects of kind event.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/kubernetes-logo.png
  humanURL: http://kubernetes.io/
  baseURL: :///api/v1beta3/127.0.0.1:6443
  tags: Containers, Google, Stack Network, API Service Provider, Containers, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/kubernetes/apiv1beta3events-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/kubernetes/apiv1beta3events-get-openapi.md
- name: Kubernetes - Get Namespaces Events
  x-api-slug: apiv1beta3namespacesnamespacesevents-get
  description: List objects of kind event.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/kubernetes-logo.png
  humanURL: http://kubernetes.io/
  baseURL: :///api/v1beta3/127.0.0.1:6443
  tags: Containers, Google, Stack Network, API Service Provider, Containers, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/kubernetes/apiv1beta3namespacesnamespacesevents-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/kubernetes/apiv1beta3namespacesnamespacesevents-get-openapi.md
- name: Kubernetes - Post Namespaces Events
  x-api-slug: apiv1beta3namespacesnamespacesevents-post
  description: Create a event.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/kubernetes-logo.png
  humanURL: http://kubernetes.io/
  baseURL: :///api/v1beta3/127.0.0.1:6443
  tags: Containers, Google, Stack Network, API Service Provider, Containers, Profiles,
    Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/kubernetes/apiv1beta3namespacesnamespacesevents-post-openapi.md
- name: Kubernetes - Delete Namespaces Events Name
  x-api-slug: apiv1beta3namespacesnamespaceseventsname-delete
  description: Delete a event.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/kubernetes-logo.png
  humanURL: http://kubernetes.io/
  baseURL: :///api/v1beta3/127.0.0.1:6443
  tags: Containers, Google, Stack Network, API Service Provider, Containers, Profiles,
    Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/kubernetes/apiv1beta3namespacesnamespaceseventsname-delete-openapi.md
- name: Kubernetes - Get Namespaces Events Name
  x-api-slug: apiv1beta3namespacesnamespaceseventsname-get
  description: Read the specified event.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/kubernetes-logo.png
  humanURL: http://kubernetes.io/
  baseURL: :///api/v1beta3/127.0.0.1:6443
  tags: Containers, Google, Stack Network, API Service Provider, Containers, Profiles,
    Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/kubernetes/apiv1beta3namespacesnamespaceseventsname-get-openapi.md
- name: Kubernetes - Put Namespaces Events Name
  x-api-slug: apiv1beta3namespacesnamespaceseventsname-put
  description: Update the specified event.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/kubernetes-logo.png
  humanURL: http://kubernetes.io/
  baseURL: :///api/v1beta3/127.0.0.1:6443
  tags: Containers, Google, Stack Network, API Service Provider, Containers, Profiles,
    Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/kubernetes/apiv1beta3namespacesnamespaceseventsname-put-openapi.md
- name: Kubernetes - Get Watch Events
  x-api-slug: apiv1beta3watchevents-get
  description: Watch a list of event.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/kubernetes-logo.png
  humanURL: http://kubernetes.io/
  baseURL: :///api/v1beta3/127.0.0.1:6443
  tags: Containers, Google, Stack Network, API Service Provider, Containers, Profiles,
    Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/kubernetes/apiv1beta3watchevents-get-openapi.md
- name: Kubernetes - Get Watch Namespaces Events
  x-api-slug: apiv1beta3watchnamespacesnamespacesevents-get
  description: Watch a list of event.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/kubernetes-logo.png
  humanURL: http://kubernetes.io/
  baseURL: :///api/v1beta3/127.0.0.1:6443
  tags: Containers, Google, Stack Network, API Service Provider, Containers, Profiles,
    Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/kubernetes/apiv1beta3watchnamespacesnamespacesevents-get-openapi.md
- name: Kubernetes - Get Watch Namespaces Events Name
  x-api-slug: apiv1beta3watchnamespacesnamespaceseventsname-get
  description: Watch a particular event.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/kubernetes-logo.png
  humanURL: http://kubernetes.io/
  baseURL: :///api/v1beta3/127.0.0.1:6443
  tags: Containers, Google, Stack Network, API Service Provider, Containers, Profiles,
    Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/kubernetes/apiv1beta3watchnamespacesnamespaceseventsname-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://knoema.api.gallery.streamdata.io
- type: x-api-stack
  url: http://kubernetes.stack.network
- type: x-blog
  url: http://blog.kubernetes.io/
- type: x-blog-rss
  url: http://blog.kubernetes.io/feeds/posts/default
- type: x-github
  url: https://github.com/kubernetes
- type: x-twitter
  url: https://twitter.com/kubernetesio
- type: x-website
  url: http://kubernetes.io/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---