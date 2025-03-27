# <div align="center">Scribd-SlideShare</div><div align="center"> ![nodedotjs](https://img.shields.io/badge/node.js-v21.6-339933.svg?style=flat&logo=nodedotjs&logoColor=white)  ![npm](https://img.shields.io/badge/npm-10.2-dc2c35.svg?style=flat&logo=npm&logoColor=white)</div>

## About ##
Scribd-SlideShare helps downloading:
- Documents on [scribd.com](https://www.scribd.com/) and [slideshare.net](https://www.slideshare.net/) --> Download files without a membership / sign-in.
- Podcast audios on [everand.com](https://www.everand.com/podcasts) --> This tool may no longer work due to Everand policy and NPM restrictions.

## Prerequisites ##
To use Scribd-SlideShare, you need to install [Node.js](https://nodejs.org/en/) and [Git](https://git-scm.com/downloads). It is recommended that you use the latest LTS version available.

> Install Node.js using pre-built installers for your device, otherwise you may encounter incompatibility issues with different development tools.

## Setup ##
1. Open Git CMD and download the repository by running this command:
```console
git clone https://github.com/CJKennedy00/scribd-slideshare
```
2. Access the necessary directory:
```console
cd ./scribd-slideshare
```
3. Install NPM:
```console
npm install
```
4. Run this command to make sure that that all possible NPM issues are fixed:
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

#### Example 1: Download 《The Minds of Billy Milligan》 on Scribd: ####
```console
npm start "https://www.scribd.com/doc/249398282/The-Minds-of-Billy-Milligan-Daniel-Keyes"
```

#### Example 2: Download 《The Minds of Billy Milligan》 using `image-based` method on Scribd: ####
```console
npm start /i "https://www.scribd.com/doc/249398282/The-Minds-of-Billy-Milligan-Daniel-Keyes"
```

#### Example 3: Download 《Everything You Need To Know About ChatGPT》 on SlideShare: ####
```console
npm start "https://www.slideshare.net/slideshow/everything-you-need-to-know-about-chatgpt-8ba3/266783915"
```

#### Example 4: Download all 《TED Talks Daily》 episodes on Everand: ####
```console
npm start "https://www.everand.com/podcast-show/414106971/TED-Talks-Daily"
```

#### Example 5: Download 《Sunday Pick: How to care for the people who take care of us (w/ Ai-jen Poo)》 on Everand: ####
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
This project is licensed under the [MIT License](LICENSE.md).
