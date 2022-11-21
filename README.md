## WhatsappStartChat Bookmarklet

This bookmarklet allows you to start chatting with any number in Whatsapp without adding it as a contact. This version only works with Whatsapp DESKTOP.
Download from Microsoft Store here: [https://www.microsoft.com/store/productId/9NKSQGP7F2NH](https://www.microsoft.com/store/productId/9NKSQGP7F2NH) 

Drag and drop the bookmarklet below to your Bookmark bar to save it. After that, click the bookmark in your browser, and a pop up will appear. Simply enter the full phone number with country code e.g. 60123456789. 

Your browser will ask you to open the link in Whatsapp Desktop. Tick the checkbox to always open in Whatsapp Desktop.

[![WA New Chat](https://i.imgur.com/AVmCJ4P.png)](javascript: { var val= prompt("Enter phone number","");} { var openChat = phone => {   const link = document.createElement("a");   link.setAttribute("href", `https://wa.me/${phone}`); document.body.append(link); link.click();   document.body.removeChild(link); }; } if (val) openChat(val))

or you can manually add the following code as a bookmark:

```
javascript: { var val= prompt("Enter phone number","");} { var openChat = phone => {   const link = document.createElement("a");   link.setAttribute("href", `https://wa.me/${phone}`); document.body.append(link); link.click();   document.body.removeChild(link); }; } if (val) openChat(val))
```
