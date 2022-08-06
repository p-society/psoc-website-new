---
title: "Getting Online"
date: 2022-03-27T17:41:25+05:30
draft: false
---

# Hugo Session Notes

## Installation

- Download the compatible .zip file from the link below
https://github.com/gohugoio/hugo/releases
(for 32-bit system - hugo_0.96.0_Windows-32bit.zip)
(for 64-bit system - hugo_0.96.0_Windows-64bit.zip)

- unzip the downloaded zip file

- open the unzipped folder and copy the location of the folder

- search for 'environment variables' and open it

- Click on 'Environment Variables' and under 'System variables' click on 'Path'

![Step-1](https://i.imgur.com/tWhqgpC.png)

then 'Edit' 

![Step-2](https://i.imgur.com/rM2keQU.png)

then 'New' 

![Step-3](https://i.imgur.com/6X0e5JA.png)

and then add the copied path.

![Step-4](https://i.imgur.com/n6yFFVN.png)

- Open powershell and type the command - `hugo version`

(If you see something like this:
```
hugo v0.96.0-2fd4a7d3d6845e75f8b8ae3a2a7bd91438967bbb windows/amd64 BuildDate=2022-03-26T09:15:58Z VendorInfo=gohugoio
```
then hugo was successfully installed on your system.

## Next Step

- ` hugo new site portfolio `
- ` cd portfolio `
- extract your fav theme in ` theme ` folder
- edit ` config.toml ` (
basically add your theme's name in 
`theme = "gohugo-theme-ananke-master"`
)
- add content to your website by ` hugo new post/firstPost `
- ` hugo server -D ` to see your site on ` http://localhost:1313 `
