# AmiBroker .NET SDK

This is yet another [AmiBroker](http://www.amibroker.com) plug-in SDK for .NET developers. As opposed to the official
C++ based [AmiBroker Development Kit](http://www.amibroker.com/download.html) (ADK) it can be used for data and/or
optimization plug-in authoring with .NET 4.5 / C#.

It is 100% free, no hidden charges, allowed for both personal and commercial use under [Apache License 2.0](http://www.apache.org/licenses/LICENSE-2.0).

Contributions of any kind are welcome! Feel free to [fork](https://github.com/kriasoft/amibroker/fork_select)
this repo and send [pull requests](https://help.github.com/articles/using-pull-requests) with your updates.

### Prerequisites

 - [Visual Studio 2012](http://www.visualstudio.com) (preferred) or Visual Studio 2010
 - [NuGet Package Manager](http://www.nuget.org) Visual Studio extension
 - [StyleCop](http://stylecop.codeplex.com/) (optional) for code style checking
 - Microsoft .NET Framework 4.5

### Community Plug-ins

 - [Yahoo Finance](http://finance.yahoo.com) real-time data plug-in for AmiBroker (planned)
 - [Finam](http://www.finam.ru) real-time data plug-in for AmiBroker (planned)

### Demo

![AmiBroker .NET SDK](http://amibroker.googlecode.com/files/Amibroker.Plugin.Screenshot.png?1)

### Getting Started

Open 'AmiBroker .NET SDK.sln' solution file in Visual Studio, update plugin information inside
`Plugin/Plugin.cs/GetPluginInfo()` method, add quotes related logic inside `Plugin/Plugin.cs/GetQuotesEx()` method,
build the project, copy "Plugin.dll" to the AmiBroker's Plugins folder or alternatively you can add a
[symbolic link](http://en.wikipedia.org/wiki/NTFS_symbolic_link) with the following command:

    mklink "C:\Program Files (x86)\AmiBroker\Plugins\Plugin.dll" "C:\Projects\AmiBroker .NET SDK\Plugin\bin\Debug\Plugin.dll"

### Support & Feedback

Visit our [discussions board](https://groups.google.com/forum/?fromgroups=#!forum/amidev), feel free to ask questions
and leave feature requests.