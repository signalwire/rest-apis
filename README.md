# SignalWire REST API Collections
SignalWire provides developers with two sets of REST APIs for managing SignalWire spaces and their associated resources: the [REST APIs](https://developer.signalwire.com/rest/) and the [Compatibility REST API](https://developer.signalwire.com/compatibility-api/rest/).
In order to streamline setup and usage, we offer pre-made collections that are compatible with Postman and Bruno.

## How to Use These Collections
SignalWire's REST APIs use authorization type [basic auth](https://www.wallarm.com/what/what-is-basic-authentication-all-you-need-to-know) where the project ID is the username and the API token is the password. The space URL is part of the base URL for every API request. These collections utilize environment variables for each of these values to simplify setup and the need for changes when swapping between projects or spaces. Authorization is set on the collection as a whole and all of the API requests inherit authorization from the collection, so you do not have to change any of these values as you use the same environment variable names.
If you do choose to use different environment variable names, be sure to update the request URLs and authentication on the collection.

You can get the required credentials [in your space](https://developer.signalwire.com/guides/navigating-your-space#api) to create the environment for each project using the names shown below:

- `Auth` -> Your API Token
- `Proj` -> Your Project ID
- `Space` -> Your Space URL (spacename.signalwire.com, no prepended https://)

## Importing Collections 
> Please note that the specific steps for importing collections into Bruno or Postman may vary based on updates to the platform or changes in its interface.
> It's always a good idea to refer to the official documentation or help resources for the most accurate and up-to-date instructions.
> - [Postman Documentation](https://learning.postman.com/docs/introduction/overview/)
> - [Bruno Documentation](https://docs.usebruno.com/)

### Postman
Postman is a very popular tool for building, testing, using, and sharing APIs. This guide focuses specifically on how to use the SignalWire collections. If you are unfamiliar with Postman or need a refresher, check out our [developer portal postman guide](https://developer.signalwire.com/apis/docs/how-to-test-api-requests-on-postman) that will explain how the tool works, how to set environment variables/environments, and how to solve common errors. 

Once you’re logged into Postman, you can click **Collections** in the sidebar and **Import** in the top right corner of the sidebar to select the downloaded collection(s).

### Bruno
While Bruno is not as widely known as Postman, it is still a powerful tool for working with APIs and can greatly streamline the process of building, testing, and using them. Bruno functions largely similarly to Postman, except that it is offline only and stores your collections directly in a folder on your file system to ensure data privacy. It also uses a [plaintext simple markup language](https://www.usebruno.com/bru), Bru, to make requests much easier to read. 

Bruno collections can be opened in two ways:

1. Click **Import Collection** to select an exported Bruno (or Postman) collection and save it locally in Bru.  
2. Click **Open Collection** to select a directory that contains the collection written in Bru.
 
To import the collection, you only need to download the JSON file in the Bruno folder for the collection you'd like to use. 

To open the collection, clone this repo and open the Bru subdirectory inside of the Bruno directory.
