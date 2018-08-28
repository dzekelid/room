---
name: TelAPI
x-slug: telapi
description: Zang offers business communications tools & voice app development platforms
  that bring innovation and ease to unified communications & collaboration solutions.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1176-telapi.jpg
x-kinRank: "9"
x-alexaRank: "1071695"
tags: Room
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/room/master/_listings/telapi/apis.md
specificationVersion: "0.14"
apis:
- name: hetras Hotel API Version 0 - Get a list with the details of all room types
    for for the specified hotel id.
  x-api-slug: apihotelv0hotelshotelidroom-types-get
  description: With this call you can load the details about a all available room
    types for the specified hotel.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1176-telapi.jpg
  humanURL: http://www.telapi.com
  baseURL: https://api.hetras-certification.net//
  tags: SMS, Voice, Voice, Target, Stack Network, Technology, SaaS, Mobile, Telecommunications,
    SMS, Telecommunications, Messages, Messages, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/room/master/_listings/telapi/apihotelv0hotelshotelidroom-types-get-openapi.md
- name: hetras Hotel API Version 0 - Get all the details for a specific room type
    in the hotel.
  x-api-slug: apihotelv0hotelshotelidroom-typescode-get
  description: With this call you can load the details about a specific room type
    in the hotel.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1176-telapi.jpg
  humanURL: http://www.telapi.com
  baseURL: https://api.hetras-certification.net//
  tags: SMS, Voice, Voice, Target, Stack Network, Technology, SaaS, Mobile, Telecommunications,
    SMS, Telecommunications, Messages, Messages, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/room/master/_listings/telapi/apihotelv0hotelshotelidroom-typescode-get-openapi.md
- name: hetras Hotel API Version 0 - Get all the details for a specific room in the
    hotel.
  x-api-slug: apihotelv0hotelshotelidroomsroomnumber-get
  description: With this call you can load the details about a specific room in the
    hotel. It will show you the current status of the room.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1176-telapi.jpg
  humanURL: http://www.telapi.com
  baseURL: https://api.hetras-certification.net//
  tags: SMS, Voice, Voice, Target, Stack Network, Technology, SaaS, Mobile, Telecommunications,
    SMS, Telecommunications, Messages, Messages, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/room/master/_listings/telapi/apihotelv0hotelshotelidroomsroomnumber-get-openapi.md
- name: hetras Hotel API Version 0 - Partially updates a room.
  x-api-slug: apihotelv0hotelshotelidroomsroomnumber-patch
  description: "The hetras API is using this Patch Specification\r\n            to
    partially update an existing resource. Currently this call only allows to modify
    condition and housekeeping occupancy status of the room.\r\n            \r\n            A
    request example:\r\n            [\r\n              {\r\n                \"op\":
    \"replace\", \"path\": \"/status/condition\", \"value\": \"CleanNotInspected\"\r\n
    \             }, {\r\n                \"op\": \"replace\", \"path\": \"/status/housekeeping_occupancy\",
    \"value\": \"Vacant\"\r\n              }\r\n            ]\r\n            \r\n
    \           For more details on how the API responds to errors please check our
    documentation on \r\n            Error Handling."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1176-telapi.jpg
  humanURL: http://www.telapi.com
  baseURL: https://api.hetras-certification.net//
  tags: SMS, Voice, Voice, Target, Stack Network, Technology, SaaS, Mobile, Telecommunications,
    SMS, Telecommunications, Messages, Messages, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/room/master/_listings/telapi/apihotelv0hotelshotelidroomsroomnumber-patch-openapi.md
x-common:
- type: x-api-gallery
  url: http://taxamo.api.gallery.streamdata.io
- type: x-api-stack
  url: http://telapi.stack.network
- type: x-base
  url: https://api.telapi.com
- type: x-blog
  url: http://www.TelAPI.com/blog/
- type: x-blog-rss
  url: http://www.telapi.com/blog/feed/
- type: x-contact-form
  url: http://www.telapi.com/contact
- type: x-crunchbase
  url: http://www.crunchbase.com/company/telapi
- type: x-crunchbase
  url: https://crunchbase.com/organization/zang-io
- type: x-developer
  url: http://www.telapi.com/docs/
- type: x-email
  url: support@telapi.com
- type: x-github
  url: https://github.com/TelAPI
- type: x-pricing
  url: http://www.telapi.com/pricing
- type: x-privacy
  url: https://www.telapi.com/legal/privacy-policy
- type: x-selfservice-registration
  url: https://www.telapi.com/signup
- type: x-status
  url: http://status.telapi.com/
- type: x-terms-of-service
  url: https://www.telapi.com/legal/tos
- type: x-twitter
  url: https://twitter.com/TelAPI
- type: x-twitter
  url: https://twitter.com/Zang_io
- type: x-website
  url: http://www.telapi.com
- type: x-website
  url: http://telapi.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---