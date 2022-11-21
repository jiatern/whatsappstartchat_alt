## WhatsappStartChat Bookmarklet

This bookmarklet allows you to start chatting with any number in Whatsapp without adding it as a contact. A pop up will appear when you click it with Whatsapp Web open.

Simple enter the full phone number with country code e.g. 60123456789.

You can drag and drop the bookmarklet below to your Bookmark bar to save it.

[![WA New Chat](https://i.imgur.com/AVmCJ4P.png)](javascript: { var val= prompt("Enter phone number","");} { var openChat = phone => {   const link = document.createElement("a");   link.setAttribute("href", `https://wa.me/6${phone}`); document.body.append(link); link.click();   document.body.removeChild(link); }; } if (val) openChat(val))

or you can manually add the following code as a bookmark:

```
javascript: { var val= prompt("Enter phone number","");} { var openChat = phone => {   const link = document.createElement("a");   link.setAttribute("href", `https://wa.me/6${phone}`); document.body.append(link); link.click();   document.body.removeChild(link); }; } if (val) openChat(val))
```
