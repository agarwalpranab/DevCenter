---
layout: tutorial
title: Setting up the MobileFirst development environment
breadcrumb_title: MobileFirst environment
relevantTo: [ios,android,windows,cordova]
weight: 1
---
## Overview
The IBM MobileFirst Platform Foundation components can be installed either seperately via online repositories which contain the latest release, or downloaded bundled together for future or offline installation using the Development Kit Installer. Continue reading to learn more about the components and how to setup the MobileFirst Development environment by following the installation guide.

> If you intend to use MobileFirst Server on IBM Containers, see the [Using Mobile Foundation](../../ibm-containers/using-mobile-foundation/) tutorial.  

#### Jump to:

* [Installation guide](#installation-guide)
* [MobileFirst Platform Foundation Development Kit](#mobilefirst-platform-foundation-development-kit)
* [MobileFirst Platform Foundation components](#mobilefirst-platform-foundation-components)
* [Applications and Adapters development](#applications-and-adapters-development)
* [Tutorials to follow next](#tutorials-to-follow-next)

## Installation guide
[Read the installation guide](installation-guide) to quickly setup MobileFirst Platform Foundation on your workstation.

## MobileFirst Platform Foundation Development Kit
The Development Kit provides a ready-for-development environment with minimal configuration needed.

The Development Kit consists of the following components: MobileFirst Server &amp; MobileFirst Operations Console, MobileFirst Developer Command-line Interface (CLI), MobileFirst client SDKs and MobileFirst adapter tooling.

### Development Kit Installer
The Installer packages the components for local installation where Internet connectivity is not available.  
The components are available through the MobileFirst Operations Console's Downloads page.

> To download the installer, visit the [downloads]({{site.baseurl}}/downloads/) page.

## MobileFirst Platform Foundation components

### MobileFirst Server
As part of the Development Kit, the MobileFirst Server is provided pre-deployed on a WebSphere Liberty profile application server. The server is pre-configured with an "mfp" runtime and uses a filesystem-based Apache Derby database.

> To download and install the MobileFirst Server, visit the [downloads]({{site.baseurl}}/downloads/) page.  

In the server directory, the following scripts are available:

* `run.[sh|cmd]`: Run the MobileFirst Server with trailing Liberty Server messages
    * Add the `-bg` flag to run the process in the background
* `stop.[sh|cmd]`: Stop the current MobileFirst Server instance
* `console.[sh|cmd]`: Open the MobileFirst Console

#### Adding the MobileFirst Server to Eclipse
The MobileFirst Server can be integrated into the Eclipse IDE.

1. From the **Servers** view in Eclipse, select **New → Server**.
2. If an IBM folder option does not exist, click on "Download additional server adapters".
3. Select **WebSphere Application Server Liberty Tools** and follow the on-screen instructions.
4. From the **Servers** view in Eclipse, select **New → Server**.
5. Select **IBM → WebSphere Application Server Liberty**.
6. Provide a server **name** and **hostname** and click **Next**.
7. Provide  the path to the server's root directory, and select a JRE version to use.
8. Click **Next** followed by clicking **Finish**.

### MobileFirst Operations Console
The MobileFirst Server's Operations Console exposes the following functionalities.  
A developer can:

- Register and deploy applications and adapters
- Optionally download native/Cordova application and adapter starter code templates 
- Configure an application's authentication and security properties
- Manage applications:
    - Application Authenticity
    - Direct Update
    - Remote Disable/Notify
- Send Push Notifications to iOS and Android devices
- Generate DevOps scripts for continuous integration workflows and faster development cycles

> Learn more about the MobileFirst Operations Console in the [Using the MobilFirst Platform Operations Console](../../setting-up-your-development-environment/console/) tutorial.

### MobileFirst Command-line Interface
The IBM MobileFirst command-line interface (CLI) tool enables developers to:

- Manage MobileFirst Servers
- Register and configure applications
- Create, build, deploy and test adapters

> To download and install the MobileFirst CLI, visit the [downloads]({{site.baseurl}}/downloads/) page.  
> Learn more about the various CLI commands in the [Using CLI to manage MobileFirst artifacts](../../using-the-mfpf-sdk/using-mobilefirst-cli-to-manage-mobilefirst-artifacts/) tutorial.

### MobileFirst Platform Foundation client SDKs and adapter tooling
MobileFirst Platform Foundation provides client SDKs for Cordova applications as well as for Native platforms (iOS, Android and Windows 8.1 Universal &amp; Windows 10 UWP). Adapter tooling for adapters and security checks development is available as well.

* To use the MobileFirst client SDKs, visit the [Adding the MobileFirst Platform Foundation SDK](../../adding-the-mfpf-sdk/) tutorials category.  
* To develop adapters, visit the [Adapters](../../adapters/) tutorials category.  
* To develop security checks, visit the [Authentication and security](../../authentication-and-security/) tutorials category.  

#### Manual installation
To use the client SDKs and adapter tooling that are provided as part of the Devlopment Kit Installer instead of the online repositories, [visit the user  documentation](http://www-01.ibm.com/support/knowledgecenter/SSHS8R_8.0.0/wl_welcome.html) for setup instructions.

## Applications and adapters development

#### Applications
* Cordova applications require NodeJS and the Cordova CLI. Read more about [setting up the Cordova development environment](../).

    You can use your preferred code editor, such as Atom.io, Visual Studio Code, Eclipse, IntelliJ and others, to implement applications and adapters.  
    
* Native applications require either Xcode, Android Studio or Visual Studio. Read more about [setting up the iOS/Android/Windows development environment](../).

#### Adapters
Adapters require Apache Maven to be installed. Refer to the [Adapters](../../adapters/) category to learn more about adapters and how to create, develop and deploy.

## Tutorials to follow next
Visit the [All Tutorials](../../all-tutorials/) page and select a tutorials category to follow next.
