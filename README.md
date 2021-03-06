# MMM-Pushbullet
> This is an extension to the [MagicMirror](https://github.com/MichMich/MagicMirror) project.  Connect to a Pushbullet stream to display notifications.

## Installation
Run these commands at the root of your magic mirror install.

```shell
cd modules
git clone https://github.com/mjtice/MMM-Pushbullet
cd MMM-Pushbullet
npm install
```

## Using the module
To use this module, add the following configuration block to the modules array in the `config/config.js` file:
```js
{
    module: 'MMM-Pushbullet',
    config: {
        // See below for configurable options
    }
}
```

### Configuration options
option | type | default | description
--- | --- | --- | ---
`api_key` | `string` | '' | The API key from Pushbullet.
`message_read_time` | `int` | 30000 | Message display timeout.
`no_message_text` | `string` | 'No new notifications' | Message to display when there are no new notifications.
`message_length` | `int` | 50 | Maximum length of characters to display for each message.
`show_message_body` | `bool` | true | Display the message body.
`number_of_messages` | `int` | 3 | Maximum number of messages to display.
