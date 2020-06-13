# Automating music downloads

This node.js script uses headless chrome browser to navigate sites and stimulate clicks.

## To use:

-   Clone and cd into the directory

```
git clone https://github.com/theParanoidScripts/automate-music-download.git && cd automate-music-download
```

-   Install dependencies like cheerio and the browser itself.<br>
    This may take a while as chromium is being downloaded into your local project.

```
npm install
```

-   Now fill in the `songs.txt` file with the music that you need downloaded.<br>
    Write the "song name [space] artist", and write each entry on each line.<br>
    Take the example `songs.txt` included in this repository for reference.

-   Now run the script

```
npm sun start
```

This will start chromium and navigate to sites.

### Note:

-   Desired extension loading with the browser is being worked upon.

-   On a related note, I do not own the website this script is using, neither do I get anything from the site owner for using it.<br>
    So please use it at your own risk.

-   Since this script uses chromium, RAM usage may be high, i.e. it will open as many tabs as the song you want to download. <br>
    If you don't want the script to crash or hang, please feed in less songs each time. This will be patched in the future.
