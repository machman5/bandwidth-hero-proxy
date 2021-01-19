![Bandwidth Hero](https://raw.githubusercontent.com/ayastreb/bandwidth-hero/master/src/assets/logo.png)

![Project CI](https://github.com/nyancodeid/bandwidth-hero-proxy/workflows/Project%20CI/badge.svg)

Bandwidth Hero is an open-source browser extension which reduces the amount of data consumed when
you browse web pages by compressing all images on the page. It uses
[data compression service](https://github.com/ayastreb/bandwidth-hero-proxy) to convert images to
low-resolution [WebP](https://developers.google.com/speed/webp/) or JPEG images.

## How It Works?

![Workflow](https://raw.githubusercontent.com/ayastreb/bandwidth-hero/master/how-it-works.png)

1. When active, Bandwidth Hero intercepts all images loading requests
2. It sends each image URL to the data compression service
3. Compression service downloads the original image
4. Once image is downloaded it is then converted to low-resolution
   [WebP](https://developers.google.com/speed/webp/)/JPEG image.
5. Compression service returns processed image to the browser

## Privacy Consideration

After installing the extension you need to setup data compression service.

Please refer to [data compression service docs](https://github.com/nyancodeid/bandwidth-hero-proxy)
for detailed instructions on how to run your own service.

Once you have your own instance running, click "Configure data compression service" button under
"Compression settings" in the extension popup.


## Deployment

### Heroku

You can deploy this service to Heroku:

[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https://github.com/nyancodeid/bandwidth-hero-proxy)

[![Deploy to Heroku guide](http://img.youtube.com/vi/y3tkYEXAics/0.jpg)](http://www.youtube.com/watch?v=y3tkYEXAics)

### Self-hosted

Data compression service is a Node.js app which you can run on any server that supports Node.js.
Check out
[this guide](https://www.digitalocean.com/community/tutorials/how-to-set-up-a-node-js-application-for-production-on-ubuntu-16-04)
on how to setup Node.js on Ubuntu.

DigitalOcean also provides an
[easy way](https://www.digitalocean.com/products/one-click-apps/node-js/) to setup a server ready to
host Node.js apps.




## Installation

[![Get Extension](https://developer.chrome.com/webstore/images/ChromeWebStore_Badge_v2_340x96.png)](https://chrome.google.com/webstore/detail/bandwidth-hero/mmhippoadkhcflebgghophicgldbahdb?hl=en-US)

[![Get Firefox Addon](https://raw.githubusercontent.com/ayastreb/bandwidth-hero/master/ff-addon-badge.png)](https://addons.mozilla.org/en-US/firefox/addon/bandwidth-hero/)

## Authors

- [ayastreb](https://github.com/ayastreb) (c) 2016 (Original) - [ayastreb/bandwidth-hero-proxy](https://github.com/ayastreb/bandwidth-hero-proxy)
- [nyancodeid](https://github.com/nyancodeid) (c) 2020 - [nyancodeid/bandwidth-hero-proxy](https://github.com/nyancodeid/bandwidth-hero-proxy)
