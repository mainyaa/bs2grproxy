# BS2 GAE Reverse Proxy

**3 Minutes to setup a mirror site!**

A small app runs on Google App Engine as a reverse proxy to a specific site, completely transparent to clients.

BS2 GAE Reverse Proxy can be used to:

- Create a mirror of a specific site to improve performance
- Break through limited network (ex. GFW)

Feel free to download or modify this program. But USE WISELY.

## BS2GRProxy Introduction

### Introduction
A small app runs on Google App Engine as a reverse proxy to a specific site.

### Features

- Reverse proxy
- Web pages, css/js and media files can be redirected to different hosts
- Configurable through Google App Database view

### How to use

1. Download the source package
2. Modify app name in app.yaml
3. Upload the app
4. Enjoy

### Configuration

You can set default config in bs2grpconfig.py. But how ever it's not encouraged to modify the source code unless you understand it.

After the first run on app engine, a data entry will be created in table "BS2GRPConfig". You can set run time options there using Data View in app admin page.

### Options in BS2GRPConfig
target_host: HTML target url.

static_host: Static target url.

cssjs_redirect: Redirect css/js files to static host. Including: .css .js

media_redirect: Redirect media files to static host. Including: .jpg .jpeg .gif .png .avi .mov .mp3 .rm .rmvb .qt

# License

GNU Lesser GPL

- Original
  - [bs2grproxy](https://code.google.com/p/bs2grproxy) by [yufeiwu](http://hi.baidu.com/ledzep2)
