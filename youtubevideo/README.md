# Display Youtube video
This extension can be used to display a youtube video:

<img src="https://github.com/artificialsolutions/teneo-web-chat-extensions/blob/master/youtubevideo/youtubevideo_screenshot.png?raw=true" width="250px">


## Installation
To install, copy the `YoutubevideoMessage.vue` file to the ` /src/components/messages/` folder of your [teneo web chat](https://github.com/artificialsolutions/teneo-web-chat) project.

## JSON
The JSON that should be included in the `teneowebclient` output parameter to display a YouTube video should look like this:
``` json
{
    "type": "youtubevideo",
    "video_url": "https://www.youtube.com/embed/IL2jOKu7LGg"
}
```

The `type` with value `youtubevideo` is used to find the appropriate `.vue` extension file. `video_url` should contain the `embed` url of the video. The embed url looks like this: `https://www.youtube.com/embed/<VIDEO ID>` where the last part should be replaced with the id of the video.
