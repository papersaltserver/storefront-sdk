# Overview of the Citrix Receiver for Web
Citrix Receiver for Web is a component of Citrix StoreFront. Citrix Receiver for Web provides access to IT resources such as Windows apps, desktops, documents, Web apps and SaaS apps, all using the Web. Citrix Receiver for Web comprises a User Interface tier (referred to as the UI tier) and a Citrix StoreFront Services Web Proxy tier (referred to as the Web Proxy). The Citrix Receiver for Web architecture is illustrated below.

![Architecture](./architecture.png)

## UI tier
The UI tier is responsible for displaying the Citrix Receiver for Web user interface and responding to user interactions. The UI tier is implemented using JavaScript/Ajax technology, loaded to and executed at the Web browser. It is divided into three areas:

* Plugin Assistant—detects whether the native HDX engine is installed and provides UI for downloading Citrix Receiver.




