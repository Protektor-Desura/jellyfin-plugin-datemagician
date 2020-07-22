<h1 align="center">Jellyfin DateMagician</h1>

<p align="center">
Jellyfin DateMagician plugin is a plugin built with .NET. </p>
<p align="center">Its main goal is to set the 'AddedDate'-Property of a TV Episode to its Premier Date to prevent the mess up of 'Latest TV Shows' in your Homescreen.
</p>

## How to use
1. Build & Install Plugin (see below)
2. Run Library Scan
3. Profit

## Build Process
1. Clone or download this repository
2. Ensure you have .NET Core SDK setup and installed
3. Build plugin with following command.
```sh
dotnet publish --configuration Release --output bin
```
4. Place the resulting .dll file in a folder called ```plugins/``` under  the program data directory or inside the portable install directory

## New Plugin Repository Support

Jellyfin 10.6.0 added the ability to have multiple repositories. So you can you can easily install and keep this plugin up to date on your server. Go to the web admin interface, select plugins on the left, then repositories at the top and click the + to create a new one using the information below.

Name:DateMagician
URL:https://raw.githubusercontent.com/Protektor-Desura/jellyfin-plugin-datemagician/master/manifest-stable.json
