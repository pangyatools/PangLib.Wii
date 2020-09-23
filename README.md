<img align="left" src=".github/Images/pang.png" width="64" />

# PangLib.Wii

[![Codacy Badge](https://app.codacy.com/project/badge/Grade/c59f8fdcfed247d6abd74ee8621f7d2a)](https://www.codacy.com/gh/pangyatools/PangLib.Wii/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=pangyatools/PangLib.Wii&amp;utm_campaign=Badge_Grade) [![Discord](https://discordapp.com/api/guilds/521180240542826496/widget.png?style=shield)](https://discord.gg/HwDTssf)

Series of tools to interact with 'Pangya: Super Swing Golf' (Wii) game files

## Usage

The libraries are built using .NET Core and .NET Standard 2.0. So you need to download and setup the [.NET Core SDK](https://www.microsoft.com/net/download) on your system.

All libraries are published on Nuget with their respective full package name, so you can install using the .NET CLI:

```shell
$ dotnet add package [package-name]
```

## Available Libraries

| Library                                       | Version                                                                                                               | Build Status                                                                                                                                                                  | Description                                              |
| --------------------------------------------- | --------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------- |
| [**PangLib.Wii.ECB**](PangLib.Wii.ECB/)       | [![Nuget](https://img.shields.io/nuget/v/PangLib.Wii.ECB.svg)](https://www.nuget.org/packages/PangLib.Wii.ECB/)       | [![Build status](https://ci.appveyor.com/api/projects/status/divi17vkamgtmqko/branch/master?svg=true)](https://ci.appveyor.com/project/pixeldesu/panglib-3511b/branch/master) | Library to handle and parse data from Wii `.ECB` files   |

## Building

To build PangLib or any of the libraries inside it, you need, just as for using it, the [.NET Core SDK](https://www.microsoft.com/net/download).

Once the SDK is available on your system to use, you can either run the following commands in the project root to build every library from the solution,
or navigate to a subfolder (e.g. `PangLib.Wii.ECB/`) and execute them there:

```
$ dotnet restore
$ dotnet build
```

If the commands run successfully, you now have compiled libraries available at `[library-name]/bin/Debug/netstandard2.0/[arch]`

To quickly test changes or use your local copy of a PangLib library in a project, you can run the following command to add 
a reference:

```
$ dotnet add reference [path to .csproj file of desired library]
```

This will now allow you to change the code of the library, and of your program and once you build your program, it will also
build the referenced library again, so you don't have to manually include a built library or publish it to Nuget yourself.

## Contributing

Want to contribute? **Awesome!**

You can contribute in many ways, like:

- Opening an issue if a problem with a library occurs.
- Opening an issue for a feature request, when a library is missing something you need.
- Opening an issue for a library request, if you need handling for another format.

Of course you can already contribute code if you are a developer, adding features, additional libraries and more, I'm
pretty open to anything, as long as it is related to Pangya and the addition is reasonable!

### Discuss on other Websites

Forum posts allowing for engagement and feedback on PangLib:

- [pangya.community](https://pangya.community/t/panglib-a-toolchain-for-pangya-files/22)
- [RageZone](http://forum.ragezone.com/f513/panglib-set-libraries-pangya-game-1162203/)

## Documentation

Documentation on the parsed file formats can be found at [docs.pangya.golf](https://docs.pangya.golf)

## License

This project is licensed under the AGPL-3.0
