# Example site: netlify-plugin-add-instagram

This site only exists to demonstrate a Netlify Build Plugin.

- Learn more about the [netlify-plugin-add-instagram](https://github.com/philhawksworth/netlify-plugin-add-instagram) plugin.
- See the example site here: https://demo-plugin-add-instagram.netlify.app


## Quick try-out

You can try out this site and its plugin out by deploying it.

Clicking the button below will clone this repo, setup a new site [on Netlify](https://netlify.com?utm_source=github&utm_medium=plugin-addinstagram-pnh&utm_campaign=devex) and deploy the site complete with the plugin configured and operational.

[![Deploy to Netlify](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/philhawksworth/demo-netlify-plugin-add-instagram&utm_source=github&utm_medium=plugin-addinstagram-pnh&utm_campaign=devex)

## Configuration

You can specify the Instagram account from which to get images by specifying the `username` in the `netlify.toml` file. Other configuration options are also available as shown below.

```toml
  [plugins.inputs]

    # Where to put the image files
    imageFolder = "src/images/instagram"

    # Also stash data about the images in a json file
    dataFile = "src/_data/instagram.json"

    # How many seconds should we cache the instagram feed for?
    feedTTL = 30

    # How many seconds should we cache each instagram image for?
    imageTTL = 1209600   # 2 weeks

    # Which of Instagrams image sizes should we fetch?
    # t (thumbnail)
    # m (medium)
    # l (large)
    imageSize = "m"

    # Instagram username
    username = "philhawksworth"
```

