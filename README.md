# SignalWire Postman Collections

Postman is a very popular tool for building, testing, using, and sharing APIs. This guide will focus specifically on how to use the SignalWire collections. If you are unfamiliar with Postman or need a refresher, check out our [developer portal postman guide](https://developer.signalwire.com/apis/docs/how-to-test-api-requests-on-postman) that will explain how the tool works, how to set environment variables/environments, and how to solve common errors. 


In this repo you'll find 2 collections:

- [Compatibility REST API](https://developer.signalwire.com/compatibility-api/rest/)
- [REST APIs](https://developer.signalwire.com/rest/)
  - Video API
  - Chat API
  - Space API
  - Message API
  - Fax API
  - Voice API

# How to Use These Collections
These collections were created with the authorization type [basic auth](https://www.wallarm.com/what/what-is-basic-authentication-all-you-need-to-know) using project ID as the username and your API token as the password. All of the API requests inherit authorization from the collection, so you do not have to do anything for auth as long as you keep the same naming in your environments. 

You can get the required credentials [in your space](https://developer.signalwire.com/guides/navigating-your-space#api) to create the environment using the names shown below: 

- Auth -> Your API Token
- Proj -> Your Project ID
- Space -> Your Space URL (spacename.signalwire.com, no prepended https://)

If you choose to use different variable names in your environment to represent the required authentication variables, you will need to change them at the collection level as well! Hover over the collection and click the three dots, then click Edit. Go to the authorization tag and adjust the environment variables to match your new names. 

