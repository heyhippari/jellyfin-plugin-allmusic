<h1 align="center">Jellyfin AllMusic Plugin</h1>
<h3 align="center">A third-party plugin for the <a href="https://jellyfin.media">Jellyfin Project</a></h3>

<p align="center">
<img alt="AllMusic plugin logo" src="https://raw.githubusercontent.com/MrTimscampi/jellyfin-plugin-allmusic/master/jellyfin-plugin-allmusic.svg?sanitize=true"/>
<br/>
<br/>
<a href="https://github.com/MrTimscampi/jellyfin-plugin-allmusic/actions?query=workflow%3A%22Test+Build+Plugin%22">
<img alt="GitHub Workflow Status" src="https://img.shields.io/github/workflow/status/MrTimscampi/jellyfin-plugin-allmusic/Test%20Build%20Plugin.svg">
</a>
<a href="https://github.com/MrTimscampi/jellyfin-plugin-allmusic">
<img alt="GPLv3 License" src="https://img.shields.io/github/license/MrTimscampi/jellyfin-plugin-allmusic.svg"/>
</a>
<a href="https://github.com/MrTimscampi/jellyfin-plugin-allmusic/releases">
<img alt="Current Release" src="https://img.shields.io/github/release/MrTimscampi/jellyfin-plugin-allmusic.svg"/>
</a>
</p>

## About

This plugin adds a metadata provider for [AllMusic](https://www.allmusic.com/).

It aims to provide the following metadata:

* Artists
  * Biography
  * Birth/formation date
  * Death/disbandment date
  * Genres
  * Images
* Albums
  * Album artist
  * Album name
  * Release date
  * Genres
  * Critics rating
  * Label
  * Images

## Installation

Add the [MrTimscampi's Plugin Emporium repository](https://github.com/MrTimscampi/jellyfin-repo) to your Jellyfin server.

## Build

1. To build this plugin you will need [.Net 5.x](https://dotnet.microsoft.com/download/dotnet/5.0).

2. Build plugin with following command
  ```
  dotnet publish --configuration Release --output bin
  ```

3. Place the dll-file in the `plugins/allmusic` folder (you might need to create the folders) of your JF installation

## Releasing

To release the plugin it is recommend to use [JPRM](https://github.com/oddstr13/jellyfin-plugin-repository-manager). It will build and package the plugin.
For additional context and for how to add the packaged plugin zip to a plugin manifest see the [JPRM documentation](https://github.com/oddstr13/jellyfin-plugin-repository-manager) for more info.

## Contributing

We welcome all contributions and pull requests! If you have a larger feature in mind please open an issue so we can discuss the implementation before you start.
In general refer to our [contributing guidelines](https://github.com/jellyfin/.github/blob/master/CONTRIBUTING.md) for further information.

## License

This plugins code and packages are distributed under the GPLv3 License. See [LICENSE](./LICENSE) for more information.
