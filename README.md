# Seletube 📺

_YouTube Playlist Downloader_. It is powered by https://loader.to/ with Selenium 4 and Microsoft Edge.

### Warning 💀

This app is only for learning purposes. I create this app because I want to learn Selenium. I tired to write the input form manually, so I learn the Selenium 4.

### How To Run 🚀

1. Let's take a look at how to install Selenium 4 with Nodejs on https://www.youtube.com/watch?v=w4cidssAdJg&list=PLZMWkkQEwOPl0udc9Dap2NbEAkwkdOTV3&index=3
2. This app uses **Microsoft Edge Driver** to run. Download a stable version https://developer.microsoft.com/en-us/microsoft-edge/tools/webdriver/
3. Extract the downloaded web driver RAR.
4. Put the location of extracted folder to your environment system (This step is also available on the video above, but the video uses Mozilla Firefox).
5. Create file `.env` and set the configuration.
6. Run the program with `npm start` or `yarn start`.

### Environment Variable 💻

The configuration of this app is available on file `.env`

#### `DOWNLOAD_FOLDER`

The folder where you want to put all downloaded files.

- Example: `C:\Users\hello\Downloads`
- Required: `true`

#### `PLAYLIST_URL`

This requires a playlist URL, not a video URL. There are different. Example screen of playlist page: https://prnt.sc/G-hMIEtwOZ_O.

- Example: `https://www.youtube.com/playlist?list=PL55RiY5tL51qLY6Yriev2bO9AF0gdvpbb`
- Required: `true`

#### `VIDEO_RES`

The resolution of video. You can check the list of resolution on https://loader.to/.

- Example: `480`
- Required: `true`

#### `CONCURRENT`

How many videos do you want to download at the same time.

- Example: `2`
- Required: `false`
- Default: `1`

#### `START`

The first position of video to download. Remember! the start is `0`.

- Example: `5`
- Required: `false`
- Default: `0`

#### `END`

The end position of video to download. The default value is total video on the playlist.

- Example: `10`
- Required: `false`
- Default: `maximum of total video`
