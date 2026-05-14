# TapMe.plus Web Publish

This repository contains the exported Godot Web build for Cloudflare Pages.

Production domain target: https://web.tapme.plus

Cloudflare Pages settings:

- Build command: leave empty
- Build output directory: /public
- Custom domain: web.tapme.plus

`large-assets/index.wasm` is intentionally kept outside the Pages output
directory because Cloudflare Pages rejects single files larger than 25 MiB.
The exported page loads it from GitHub raw at runtime.

Source project: https://github.com/wanmeixx/TapMe-1-Godot
