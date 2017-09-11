# Imagine

[![build](https://travis-ci.org/meowtec/Imagine.svg?branch=master)](https://travis-ci.org/meowtec/Imagine)

Imagine is a desktop app for compression of PNG and JPEG, with a modern and friendly UI.

Save for web.

## Install

For Windows, macOS and Linux, download binaries from:

[https://github.com/meowtec/Imagine/releases](https://github.com/meowtec/Imagine/releases)

国内用户从 GitHub 下载可能比较慢，可以使用[国内加速](https://github.com/meowtec/Imagine/issues/7)

### Install on linux

App for linux is distributed in [AppImage](http://appimage.org/) format.
Install it with command line:

```bash
chmod a+x Imagine-[v]-x86_64.AppImage # make executable
./Imagine-[v]-x86_64.AppImage # install and run
```

## Screenshot (from legacy version)

[GIF(7.4M)](http://7qn7vf.com1.z0.glb.clouddn.com/IMAGINE2.gif)

![](http://7qn7vf.com1.z0.glb.clouddn.com/Imagine.png)

## Features

 - Multi format (JPEG, PNG, WebP)
 - Format conversion
 - Cross platform
 - GUI
 - Batch optimization
 - i18n (English, 简体中文, Nederlands, español, Français)

## 'ImageMagick required'

Since version 0.3.0, you can choose the format that you want to convert to. For example, if you pick a PNG file, you can convert it to JPEG and compress it with MozJPEG optimizer.

But there is an exception: pngquant on windows can't read JPEG files, so if you want to convert JPEG to PNG, you should install ImageMagick firstly, and add it to your PATH environment variable.

## Build and Contribute

```bash
git clone https://github.com/meowtec/Imagine.git
# node 8 is recommended
npm install
npm run dev
```

A PR with **all checks passed** is welcome.

Before submit a PR, please run `npm run test` and make sure it success on your machine.

Up to now, there are only [5 locales](https://github.com/meowtec/Imagine/tree/dev/modules/locales). To add a new locale, you can either submit a PR, or [create an issue](https://github.com/meowtec/Imagine/issues/new), or just send me an email(found in [my profile](https://github.com/meowtec)).

## Built on

 - [pngquant](https://pngquant.org/): Lossy PNG compressor
 - [mozjpeg](https://github.com/mozilla/mozjpeg): Improved JPEG encoder
 - [WebP](https://developers.google.com/speed/webp/): A new image format for the Web
 - [Electron](https://electron.atom.io/): Build cross platform desktop apps with JavaScript, HTML, and CSS
