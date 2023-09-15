<div align=center>
<p align=center><img src=https://user-images.githubusercontent.com/27947066/267328833-3e81a98e-2acb-4291-89cb-f3f9bed6c299.png width=250px></p>
<h1 align=center> RADIO-ACTIVE </h1>

<p align=center> Play any radios around the globe right from your terminal </p>

<a href="https://www.producthunt.com/posts/radio-active?utm_source=badge-featured&utm_medium=badge&utm_souce=badge-radio-active" target="_blank"><img src="https://api.producthunt.com/widgets/embed-image/v1/featured.svg?post_id=305380&theme=dark" alt="radio-active - Play more than 30K radio stations from your terminal | Product Hunt" style="width: 250px; height: 54px;" width="250" height="54" /></a>

 <p align=center ><img align=center src=https://static.pepy.tech/personalized-badge/radio-active?period=total&units=international_system&left_color=black&right_color=green&left_text=TotalInstalls></p> 
 <p>
<img width="500px" alt="UPI" src="https://user-images.githubusercontent.com/27947066/235618869-8c9d9bce-096d-469e-8f61-c29cc01eacc3.png">
</p>

<p align=center>
<img align=center src=https://github.com/deep5050/random-shits-happen-here/assets/27947066/250dcd05-c142-442a-a9a3-66347adb69c5 >
<hr>
<img alt="GitHub" src="https://img.shields.io/github/license/deep5050/radio-active?style=for-the-badge">
<img alt="PyPI" src="https://img.shields.io/pypi/v/radio-active?style=for-the-badge">
<img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dm/radio-active?style=for-the-badge">
<img alt="CodeFactor Grade" src="https://img.shields.io/codefactor/grade/github/deep5050/radio-active/main?style=for-the-badge">
<a href=https://discord.gg/53rfebFyqK><img alt="Discord" src="https://img.shields.io/discord/847703568949051392?style=for-the-badge"></a>
</p>

<p align=center> <a href=https://www.youtube.com/watch?v=X-NfK5XbM90><img alt="YouTube Video Likes and Dislikes" src="https://img.shields.io/youtube/likes/X-NfK5XbM90?style=social&withDislikes"></a></p>
<p align=center> <a href=https://discord.gg/53rfebFyqK> Join Discord Server </a></p>

</div>

### Features

- [x] Supports more than 30K stations !!
- [x] Saves last station information
- [x] Favorite stations (Aliasing)
- [x] Supports user-added stations
- [x] Looks minimal and user-friendly
- [x] Runs on Raspberry-Pi
- [x] Finds nearby stations
- [x] Discovers stations by genre
- [x] Discovers stations by language
- [ ] I'm feeling lucky ! Play Random stations


> See my progress [here](https://github.com/deep5050/radio-active/projects/1)


### External Dependency

It needs [FFmpeg](https://ffmpeg.org/download.html) to be installed on your
system in order to play the audio

on Ubuntu based system >= 20.04 Run

```
sudo apt update
sudo apt install ffmpeg
```

For other systems including windows see the above link

#### Installing FFmpeg

FFmpeg is required for this program to work correctly. Install FFmpeg by following these steps :-

- On Linux - <https://www.tecmint.com/install-ffmpeg-in-linux/>
- On Windows - <https://www.wikihow.com/Install-FFmpeg-on-Windows>


### Install

Just run: `pip3 install --upgrade radio-active`

I encourage you to install with pipx: `pipx install radio-active`

### Run

Run with `radioactive --station [STATION_NAME]` or as simply `radio -U [UUID] ` :zap:

### Tips

1. Use a modern terminal emulator, otherwise the UI might break! (gets too ugly sometimes)
2. On Windows, instead of default Command Prompt, use the new Windows Terminal or web-based emulators like hyper,Cmdr,Terminus etc. for better UI
3. Let the app run for at least 5 seconds (not a serious issue though, for better performance)


### Demo

<a align=center href="https://www.youtube.com/watch?v=X-NfK5XbM90" target="_blank"> <img align=center src=https://user-images.githubusercontent.com/27947066/267328820-f7264e02-edc1-46f3-9548-5dfb50a6627d.jpg /> </a>
<hr>
<a align=center href="https://asciinema.org/a/412285" target="_blank"><img src="https://asciinema.org/a/412285.svg" /></a>



### Options


| Argument                     | Note                                | Description                                  | Default |
| ---------------------------- | ----------------------------------- | -------------------------------------------- | ------- |
| `--station`, `-S`            | Required (Optional from second run) | Station name                                 | None    |
| `--uuid`, `-U`               | Optional                            | ID of the station                            | None    |
| `--log-level`, `-L`          | Optional                            | Log level of the program                     | Info    |
| `--add-station` , `-A`       | Optional                            | Add an entry to fav list                     | False   |
| `--show-favorite-list`,`-W`  | Optional                            | Show fav list                                | False   |
| `--add-to-favorite`,`-F`     | Optional                            | Add current station to fav list              | False   |
| `--flush`                    | Optional                            | Remove all the entries from fav list         | False   |
| `--discover-by-country`,`-D` | Optional                            | Discover stations by country code            | False   |
| `--discover-by-state`        | Optional                            | Discover stations by country state           | False   |
| `--discover-by-tag`          | Optional                            | Discover stations by tags/genre              | False   |
| `--discover-by-language`     | optional                            | Discover stations by                         | False   |
| `--limit`                    | Optional                            | Limit the # of results in the Discover table | 100     |
| `--volume`                   | Optional                            | Change the volume passed into ffplay         | 80      |
| `--kill`                     | Optional                            | Kill background radios.                      | False   |

<hr>


> `--station`, `-S` : Expects a station name to be played (if not provided it
> will try to get the last played station). Example: "pehla nasha" ,
> pehla_nasha, bbc_radio

> `--uuid`,`-U` : When station names are too long or confusing (or multiple
> results for the same name) use the station's uuid to play . --uuid gets the
> greater priority than --station. Example: 96444e20-0601-11e8-ae97-52543be04c81

> `--log-level`, `-L` : don't need to specify unless you are developing it. `info` , `warning` , `error` , `debug` 

> `-F` : Add current station to your favorite list. Example: `-F my_fav_1`

> `-A`: Add any stations to your list. You can add stations that are not currently available on our API. When adding a new station enter a name and direct URL to the audio stream. 


### Changes

see [CHANGELOG](./CHANGELOG.md)

### Community

Share you favorite list with our community 🌐 ➡️ [Here](https://github.com/deep5050/radio-active/discussions/10)

> Your favorite list `.radio-active-alias` is under your home directory as a hidden file :)

### Extra

If you ever face a situation where radio-active quits but the audio (ffplay) runs in the background. Kill the process ID (PID) of ffplay. Run `ps -al` get the PID of ffplay and `kill [PID]`. I know you Know that :)


### Support

<p> 
<a href=https://deep5050.github.io/payme>Visit my contribution page for more payment options.
</p>
<p align=center><a href="https://www.buymeacoffee.com/deep5050" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me A Coffee" style="height: 40px !important;width: 117px !important;" ></a></p>

### Acknowledgements

<div>Icons made by <a href="https://www.freepik.com" title="Freepik">Freepik</a> from <a href="https://www.flaticon.com/" title="Flaticon">www.flaticon.com</a></div>


<div align=center>
<img src=https://github.com/deep5050/random-shits-happen-here/assets/27947066/83d08065-c209-4012-abb7-9c0aa64d761b width=400px >
<p align=center> Happy Listening </p>

</div>


## Contributors ✨

Thanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):

<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
<!-- prettier-ignore-start -->
<!-- markdownlint-disable -->
<table>
  <tbody>
    <tr>
      <td align="center" valign="top" width="14.28%"><a href="http://www.bjoli.com"><img src="https://avatars.githubusercontent.com/u/48383?v=4?s=100" width="100px;" alt="Joe Smith"/><br /><sub><b>Joe Smith</b></sub></a><br /><a href="https://github.com/deep5050/radio-active/commits?author=Yasumoto" title="Tests">⚠️</a> <a href="https://github.com/deep5050/radio-active/commits?author=Yasumoto" title="Code">💻</a> <a href="#ideas-Yasumoto" title="Ideas, Planning, & Feedback">🤔</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/salehjafarli"><img src="https://avatars.githubusercontent.com/u/81613563?v=4?s=100" width="100px;" alt="salehjafarli"/><br /><sub><b>salehjafarli</b></sub></a><br /><a href="https://github.com/deep5050/radio-active/commits?author=salehjafarli" title="Code">💻</a></td>
    </tr>
  </tbody>
</table>

<!-- markdownlint-restore -->
<!-- prettier-ignore-end -->

<!-- ALL-CONTRIBUTORS-LIST:END -->

This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!

<div align=center>
<p>
<img src=https://stars.medv.io/deep5050/radio-active.svg align=center>
</p>
</div>