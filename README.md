**_This bot made for testing powerful abilities of node-red platform in bot-developing

- Language - Russian, but all nodes have english-localization name.
- Contains his own Database on Sqlite server
- Using an imgur.com hosting to save images. 

**IMPORTANT

!!Make a .db file with name "UserInfoDB" and make tables inside with "inject" button on the node-red dashboard.
!!To work properly you need a database, which is in a rep. with name Database.db
!!Need an Environment file to work.
!!Make a text document with this context and convert it to .bat

Example of Environment file:

=======-----==============-----==============-----==============-----==============-----=======

@ECHO OFF
set TOKEN_VIBER=*your token*
set NGROK_VIBER=*ngrok tunnel*/viber_bot
set VIBER_SET_WEBHOOK=https://chatapi.viber.com/pa/set_webhook
set VIBER_SEND_MESSAGE=https://chatapi.viber.com/pa/send_message
set TOKEN_TELEGRAM=*your token*
set NGROK_TELEGRAM=*ngrok tunnel*/telegram_bot
set TELEGRAM_EDIT_MESSAGE=https://api.telegram.org/bot%TOKEN_TELEGRAM%/editMessageText
set TELEGRAM_CALLBACK_ANSWER=https://api.telegram.org/bot%TOKEN_TELEGRAM%/answerCallbackQuery
set TELEGRAM_SET_WEBHOOK=https://api.telegram.org/bot%TOKEN_TELEGRAM%/setWebhook?url=%NGROK_TELEGRAM%
set TELEGRAM_SEND_MESSAGE=https://api.telegram.org/bot%TOKEN_TELEGRAM%/sendMessage
set TELEGRAM_SEND_PHOTO=https://api.telegram.org/bot%TOKEN_TELEGRAM%/sendPhoto
node-red

=======-----==============-----==============-----==============-----==============-----=======

Short description:

Bot(for ShoeMarket) with autorization and sync between two messengers(Viber and Telegram). Made not for commerce.

Requirements:

node-red-node-sqlite
node-red version upper 1.2.3,
node.js version upper 12.13.0
npm ci (in main branch)

© Nassar.K - 2020
