---
title: AddText Limitation
page_title: AddText Limitation | UI for ASP.NET AJAX Documentation
description: AddText Limitation
slug: imageeditor/troubleshooting/known-issues/addtext-limitation
tags: addtext,limitation
published: True
position: 1
---

# AddText Limitation



## 

There is a known limitation in __RadImageEditor__'s __AddText__ tool.

The __AddText__ tool inserts the text to the image currently saved on the server. If any client-side operations are performed, such as Rotate, Flip, or Resize, and they are not applied on the server, the text will be added without taking into consideration the current client state of the image. To be sure that the text is added correctly please apply all changes to the image on the server.

Example of how the __AddText__ tool does not respect the client operations performed up to now:

1. Original image
>caption 

![radimageeditor-add-text-limitation-im 1](images/radimageeditor-add-text-limitation-im1.jpg)

1. We rotate the image
>caption 

![radimageeditor-add-text-limitation-im 2](images/radimageeditor-add-text-limitation-im2.jpg)

1. We AddText
>caption 

![radimageeditor-add-text-limitation-im 3](images/radimageeditor-add-text-limitation-im3.jpg)

1. Result
>caption 

![radimageeditor-add-text-limitation-im 4](images/radimageeditor-add-text-limitation-im4.jpg)