# Display Clickable List
This extension can be used to display a list of clickable items:

![Clickable list example](clickablelist_example.png | width=100)

## Installation
To install, copy the `ClickablelistMessage.vue` file to the ` /src/components/messages/` folder of your teneo web chat project.

## JSON
The JSON that should be including in the `teneowebclient` output parameter to display a list of clickable items should look like this:
``` json
{
    "type": "clickablelist",
    "list_items": [
        {
            "title": "Gouda",
            "postback": "Gouda"
        },
        {
            "title": "Brie",
            "postback": "Brie"
        },
        {
            "title": "American Cheese",
            "postback": "American Cheese"
        },
        {
            "title": "Pecorino Romano",
            "postback": "Pecorino Romano"
        },
        {
            "title": "Cheddar",
            "postback": "Cheddar"
        },
        {
            "title": "Manchego",
            "postback": "Manchego"
        },
        {
            "title": "Camembert",
            "postback": "Camembert"
        }
    ]
}
```

The `type` with value `clickablelist` is used to find the appropriate `.vue` extension file. The `list_item` should contain an list of item. For each item, the `title` is displayed in the list and the `postback` value is sent back to the teneo engine when the user selects the item.