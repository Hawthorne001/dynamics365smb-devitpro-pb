---
title: Developing extensions in AL
description: Overview of the development experience for building extensions using the AL language.
author: SusanneWindfeldPedersen
ms.date: 04/01/2025
ms.topic: overview
ms.author: solsen
ms.collection: get-started
ms.reviewer: solsen
---

# Development in AL

[!INCLUDE [getstarted-contributions](includes/getstarted-contributions.md)]

Extensions are a programming model where functionality is defined as an addition to existing objects and defines how they're different or modify the behavior of the solution. This section explains how you can develop extensions using the development environment for [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)].

If you're new to building extensions, we recommend that you read this document to get an understanding of the basics and terms you encounter while working. Next, follow the [Get Started with AL](devenv-get-started.md) to set up the tools.

## Understanding objects in the development environment

All functionality in [!INCLUDE[prod_short](includes/prod_short.md)] is coded in objects. The extension model is object-based; you create new objects, and extend existing objects depending on what you want your extension to do.

- Table objects define the table schema that holds data.
- Page objects represent the pages seen in the user interface.
- Codeunits contain code for logical calculations and for the application behavior.
- Report objects define the layout and data for reports.

Learn more about the objects that you can create for your extension in [Extension objects overview](devenv-extension-object-overview.md).

These objects are stored as code, known as AL code, and are saved in files with the `.al` file extension. The [!INCLUDE[d365al_ext_md](../includes/d365al_ext_md.md)] also supports the multi-root functionality, which allows you to work with multiple AL folders within one workspace. Learn more about how to group a set of disparate project folders into one workspace in [Working with multiple AL project folders within one workspace](devenv-multiroot-workspaces.md).

> [!NOTE]  
> A single .al file might contain multiple objects, however, it's a best practice to have one object per file.

Table extension objects and page extension objects are used to add or override changes to table or page objects. For example, consider a business that sells organic food, and the business wants to add two extra fields; `Organic` and `Local Produce` in its existing item table. The business uses a table extension object to define those extra fields. The table extension makes the newly added fields available for use in the item table. You can store data in these fields and access them by code. You can then use the page extension object to display the fields in the UI.

> [!NOTE]  
> Extension objects can have a name with a maximum length of 30 characters.

You have several options for creating new objects with the [!INCLUDE[d365al_ext_md](../includes/d365al_ext_md.md)] for Visual Studio Code. Learn more about the objects that you can create for your extension in [AL development environment](devenv-reference-overview.md).

## Developing extensions in Visual Studio Code

Using the [!INCLUDE[d365al_ext_md](../includes/d365al_ext_md.md)] for Visual Studio Code, you get the benefits of a modern development environment along with seamless publishing and integration with your [!INCLUDE[prod_short](includes/prod_short.md)] tenant. Learn more about the setup in [Get started with AL](devenv-get-started.md).

Visual Studio Code and the [!INCLUDE[d365al_ext_md](../includes/d365al_ext_md.md)] let you do the following tasks:

- Create new files for your solution.
- Assists you with the creation of appropriate settings and configuration files.
- Provides code snippets to help create application objects.
- Gives compiler validation while you code.
- Provides efficient publishing process. You can publish and see your code running by just selecting <kbd>Ctrl</kbd>+<kbd>F5</kbd>.

> [!NOTE]
> For some users the <kbd>Ctrl</kbd>+<kbd>F5</kbd>  shortcut key might not work due to keyboard or other settings. If it doesn't work for you, run your code by choosing **Run Without Debugging** from the **Run** menu in Visual Studio Code.  

[!INCLUDE[intelli_shortcut](includes/intelli_shortcut.md)]

## Extending the functionality of Business Central

You can extend the functionality of Business Central in several ways: you can extend tables, enumerations, application areas, pages, reports, code flows, and the security model directly in AL. But you can also contribute directly to the base application in the open source projects for the system application modules.

Learn more about the extensibility options available to AL developers in [!INCLUDE[prod_short](../developer/includes/prod_short.md)] including examples on how to extend various features, such as extending item charges, best price calculations, and data archiving in [Extensibility overview](devenv-extensibility-overview.md).

## Designer

Designer works in the client and allows you to design pages using drag and drop components. Designer lets you build extensions in the client itself by rearranging fields, adding fields, and previewing your changes in page design. Learn more in [Use Designer](devenv-inclient-designer.md).

## Compiling and deploying

Extensions are compiled as .app package files. The .app package file can be deployed to the [!INCLUDE[prod_short](includes/prod_short.md)] server. A .app package contains the various artifacts that deliver the new functionality to the [!INCLUDE[prod_short](includes/prod_short.md)] deployment and a manifest that specifies the name, publisher, version, and other attributes of the extension. Learn more about the manifest files in [JSON files](devenv-json-files.md).

## Instrumenting your app with telemetry

[!INCLUDE[prod_short](includes/prod_short.md)] emits telemetry data for several operations that occur when extension code is run. You can configure your extension to send this data to a specific Application Insights resource on Microsoft Azure. Learn more in [Sending extension telemetry to Azure Application Insights](devenv-application-insights-for-extensions.md).

## Submitting your app

After development and testing are done, you can submit your extension package to AppSource. Before you submit the extension package, we encourage you to read the checklist to facilitate the validation process. Learn more in [Checklist for submitting your app](devenv-checklist-submission.md). To get code validation helping you to bring your extension package to AppSource, you can enable the AppSourceCop code analyzer. Learn more in [Using the code analysis tool](devenv-using-code-analysis-tool.md).

## Related information

[Get started with AL](devenv-get-started.md)  
[Get started developing Connect apps for Dynamics 365 Business Central](devenv-develop-connect-apps.md)  
[Keyboard shortcuts](devenv-keyboard-shortcuts.md)  
[AL development environment](devenv-reference-overview.md)  
[Documenting your code with XML comments](devenv-xml-comments.md)  
[FAQ for developing in AL](devenv-dev-faq.md)  
[Sending extension telemetry to Azure Application Insights](devenv-application-insights-for-extensions.md)  
