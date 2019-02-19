# Teneo Web Chat Extensions

This repository contains optional extensions that can be used to extend the functionality of the [Teneo Web Chat](https://github.com/artificialsolutions/teneo-web-chat) example GUI.


## Extending

The web chat UI can be extended by adding the `.vue` file for an extension in the [/src/components/messages/](/src/components/messages/) folder. This file should parse the JSON that is included in an output parameter called `teneowebclient` in the engine response. The .vue file should  display the data accordingly.


### Using an extension

To add an extensions from this repository to your project, proceed as follows:

1. Copy the `.vue` file to the `/src/components/messages/` folder of you project.
2. Create an example flow in Teneo Studio that includes the appropriate JSON in the output parameter `teneowebclient` and publish your solution. The JSON is specified in the extension's Readme file.
3. Test the result by connecting your web chat UI to the the engine with the example flow.



