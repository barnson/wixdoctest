---
sidebar_position: 10
---

# About

The WiX Toolset lets developers create installers for Windows Installer,
the Windows installation engine.

* The core of WiX is a set of build tools that build Windows Installer packages
  using the same build concepts as the rest of your product: source code is compiled
  and then linked to create executables; in this case .exe setup bundles, .msi installation
  packages, .msm merge modules, and .msp patches. The WiX command-line build tools
  work with any automated build system. Also, MSBuild is supported from the command
  line, Visual Studio, and common CI/CD build systems like GitHub Actions.

* WiX includes several extensions that offer functionality beyond that of Windows
  Installer. For example, WiX can install IIS web sites, create SQL Server databases,
  and register exceptions in the Windows Firewall, among others.

* With Burn, the WiX bootstrapper, you can create setup bundles that install prerequisites
  like the .NET Framework and other runtimes along with your own product. Burn lets
  you download packages or combine them into a single downloadable .exe.

* The WiX SDK includes managed and native libraries that make it easier to write
  code that works with Windows Installer, including custom actions in both C# and
  C++.

You can also follow via Twitter <a href="https://twitter.com/wixtoolset" class="twitter-follow-button" data-show-count="true" data-lang="en">at @wixtoolset</a>
