# About

DX Launcher is an utility application to manage your installed Rock Band 3 song packages and download new ones by the MiloHasx community! This repository acts as a public database of song packages for Rock Band 3, fetched automatically by DX Launcher!

# JSON Structure

If you want to contribute and add your own song packages, just add a new entry on the `packages` array on `packages.json` file and create a pull request. This file will be fetched by DX Launcher every time you open it to display new packs!

Here's the structure of an entry:

| KEY          | VALUE TYPE | DESCRIPTION                                                                                                        | REQUIRED |
|--------------|------------|--------------------------------------------------------------------------------------------------------------------|----------|
| name         | `string`   | The name of the song package.                                                                                      | &check;  |
| version      | `number`   | The version of the song package.                                                                                   | &check;  |
| hash         | `string`   | The hash of the song package.                                                                                      | &check;  |
| fileSize     | `string`   | The file size of the song package. Must always be the file size of the Xbox 360 CON file format.                   | &check;  |
| songsCount   | `number`   | The number of the songs inside the song package.                                                                   | &check;  |
| dta          | `url`      | The URL of the `songs.dta` file inside the song package.                                                           | &check;  |
| thumbnail    | `url`      | The URL of the song package artwork.<br />_Preffered format and size: WEBP format, 256x256 pixels_.                | &check;  |
| description  | `url`      | A description file in Markdown `.md` file format.                                                                  | &check;  |
| downloadXbox | `url`      | The Download URL of your song package in Xbox 360 CON Format.                                                      | &check;  |
| downloadPS3  | `url`      | The Download URL of your song package in PS3 PKG Format.                                                           | &check;  |
| downloadWii  | `url`      | The Download URL of your song package in Wii Format (Meta and Song folders), compressed in `.zip` or `.7z` format. |          |
