---
title: "messages.setChatWallPaper"
description: "Set a custom [wallpaper »](https://core.telegram.org/api/wallpapers) in a specific private chat with another user."
grand_parent: "Telegram RPC API"
parent: "Methods"
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
redirect_from: /API_docs/methods/messages_setChatWallPaper.html
---
# Method: messages.setChatWallPaper
[Back to methods index](index.html)



Set a custom [wallpaper »](https://core.telegram.org/api/wallpapers) in a specific private chat with another user.

### Parameters:

| Name     |    Type       | Description | Required |
|----------|---------------|-------------|----------|
|peer|[Username, chat ID, Update, Message or InputPeer](/API_docs/types/InputPeer.html) | The private chat where the wallpaper will be set | Optional|
|wallpaper|[InputWallPaper](/API_docs/types/InputWallPaper.html) | The [wallpaper »](https://core.telegram.org/api/wallpapers), obtained as described in the [wallpaper documentation »](https://core.telegram.org/api/wallpapers#uploading-wallpapers); must **not** be provided when installing a wallpaper obtained from a [messageActionSetChatWallPaper](../constructors/messageActionSetChatWallPaper.html) service message (`id` must be provided, instead). | Optional|
|settings|[WallPaperSettings](/API_docs/types/WallPaperSettings.html) | Wallpaper settings, obtained as described in the [wallpaper documentation »](https://core.telegram.org/api/wallpapers#uploading-wallpapers) or from [messageActionSetChatWallPaper](../constructors/messageActionSetChatWallPaper.html).`wallpaper`.`settings`. | Optional|
|id|[int](/API_docs/types/int.html) | If the wallpaper was obtained from a [messageActionSetChatWallPaper](../constructors/messageActionSetChatWallPaper.html) service message, must contain the ID of that message. | Optional|


### Return type: [Updates](/API_docs/types/Updates.html)

### Can bots use this method: **YES**


### MadelineProto Example ([now async for huge speed and parallelism!](https://docs.madelineproto.xyz/docs/ASYNC.html)):


```php
if (!file_exists('madeline.php')) {
    copy('https://phar.madelineproto.xyz/madeline.php', 'madeline.php');
}
include 'madeline.php';

$MadelineProto = new \danog\MadelineProto\API('session.madeline');
$MadelineProto->start();

$Updates = $MadelineProto->messages->setChatWallPaper(peer: $InputPeer, wallpaper: $InputWallPaper, settings: $WallPaperSettings, id: $int, );
```

