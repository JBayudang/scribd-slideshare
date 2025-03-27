# <div align="center">Scribd-SlideShare</div><div align="center"> ![nodedotjs](https://img.shields.io/badge/node.js-v21.6-339933.svg?style=flat&logo=nodedotjs&logoColor=white)  ![npm](https://img.shields.io/badge/npm-10.2-dc2c35.svg?style=flat&logo=npm&logoColor=white)</div>

## About ##
Scribd-SlideShare helps downloading:
- documents on [scribd.com](https://www.scribd.com/) and [slideshare.net](https://www.slideshare.net/) without membership / sign-in  
- podcast audios on [everand.com](https://www.everand.com/podcasts)  

## Prerequisites ##
To use Scribd-SlideShare, you need to install [Node.js](https://nodejs.org/en/) and [Git](https://git-scm.com/downloads). It is recommended that you use the latest LTS version available.  

> Install Node.js using pre-built installers for your device, otherwise you may encounter incompatibility issues with different development tools.  

To check that Node.js was installed correctly, type the this command in your terminal client
```console
node -v && npm -v
```
The command should print the versions of both Node.js and npm.  

## Setup ##
1. Download this repository  
```console
git clone https://github.com/CJKennedy00/scribd-slideshare
```
2. Open directory
```console
cd ./scribd-slideshare
```
3. Install dependencies
```console
npm install
```
4. Run this command to make sure that that all possible NPM issues are fixed
```console
npm audit fix --force
```

## Usage (CLI) ##
```console
DEFAULT: npm start url
        PDF-Based Files: Output files will be in PDF.

* OPTIONAL: npm start /i url
        Image-Based Files: Output files will be in image format instead of PDF. Can only be used when downloading files from Scribd.
```

#### Example 1: Download 《The Minds of Billy Milligan》 on scribd.com ####
```console
npm start "https://www.scribd.com/doc/249398282/The-Minds-of-Billy-Milligan-Daniel-Keyes"
```

#### Example 2: Download 《The Minds of Billy Milligan》 using `image-based` method on scribd.com ####
```console
npm start /i "https://www.scribd.com/doc/249398282/The-Minds-of-Billy-Milligan-Daniel-Keyes"
```

#### Example 3: Download 《Everything You Need To Know About ChatGPT》 on slideshare.net ####
```console
npm start "https://www.slideshare.net/slideshow/everything-you-need-to-know-about-chatgpt-8ba3/266783915"
```

#### Example 4: Download all 《TED Talks Daily》 episodes on everand.com ####
```console
npm start "https://www.everand.com/podcast-show/414106971/TED-Talks-Daily"
```

#### Example 5: Download 《Sunday Pick: How to care for the people who take care of us (w/ Ai-jen Poo)》 on everand.com ####
```console
npm start "https://www.everand.com/listen/podcast/731670963"
```

## Support URL Format ##
- https://www.scribd.com/doc/
- https://www.scribd.com/embeds/
- https://www.slideshare.net/
- https://www.slideshare.net/slideshow/
- https://www.everand.com/podcast-show/
- https://www.everand.com/podcast/
- https://www.everand.com/listen/podcast/

## Development Plan ##
- Scribd obfuscates the .pdf files, the texts copied from the documents might become strange garbled message. De-obfuscating is one of my future plans.

## License ##
This project is licensed under the [MIT License](LICENSE.md)
