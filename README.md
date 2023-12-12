[![Latest stable version]][packagist] [![Total downloads]][packagist] [![License]][packagist] [![GitHub forks]][fork] [![Donate Paypal]][paypal] [![Wishlist amazon]][amazon] [![GitHub stars]][stargazers] [![GitHub watchers]][subscription] [![GitHub followers]][followers] [![Follow Jon on Twitter]][twitter]

# Jonnitto.PrettyEmbedVideoStreaming

**For a detail guide, please visit the [PrettyEmbed Wiki](https://github.com/jonnitto/Jonnitto.PrettyEmbedHelper/wiki)**

Prettier embeds for your native streaming videos in [Neos CMS] - with excellent options like high-res preview images,
lightbox feature, captions, and advanced customization of embed options.

![Screenshot]

| Version | Neos         | Maintained |
| ------- | ------------ | :--------: |
| 1.\*    | 4.2.\*, >= 5 |     ✗      |
| 2.\*    | >= 5.3       |     ✗      |
| 6.\*    | >= 7.3       |     ✓      |

> The version jump was made to have all packages from the PrettyEmbed series on the same number

## Installation

Most of the time, you have to make small adjustments to a package (e.g., configuration in `Settings.yaml`). Because of
that, it is essential to add the corresponding package to the composer from your theme package. Navigate to this package
in your CLI and run the following command:

```bash
composer require jonnitto/prettyembedvideostreaming --no-update
```

The `--no-update` command prevent the automatic update of the dependencies. After the package was added to your package
`composer.json`, go back to the root of the Neos installation and run `composer update`. Et voilà! Your desired package
is now installed correctly.

[screenshot]: https://github.com/jonnitto/Jonnitto.PrettyEmbedVideoStreaming/assets/4510166/c2e52805-4990-468f-b2ed-11de28aefc14
[packagist]: https://packagist.org/packages/jonnitto/prettyembedvideostreaming
[latest stable version]: https://poser.pugx.org/jonnitto/prettyembedvideostreaming/v/stable
[total downloads]: https://poser.pugx.org/jonnitto/prettyembedvideostreaming/downloads
[license]: https://poser.pugx.org/jonnitto/prettyembedvideostreaming/license
[github forks]: https://img.shields.io/github/forks/jonnitto/Jonnitto.PrettyEmbedVideoStreaming.svg?style=social&label=Fork
[donate paypal]: https://img.shields.io/badge/Donate-PayPal-yellow.svg
[wishlist amazon]: https://img.shields.io/badge/Wishlist-Amazon-yellow.svg
[amazon]: https://www.amazon.de/hz/wishlist/ls/2WPGORAVYF39B?&sort=default
[paypal]: https://www.paypal.me/Jonnitto/20eur
[github stars]: https://img.shields.io/github/stars/jonnitto/Jonnitto.PrettyEmbedVideoStreaming.svg?style=social&label=Stars
[github watchers]: https://img.shields.io/github/watchers/jonnitto/Jonnitto.PrettyEmbedVideoStreaming.svg?style=social&label=Watch
[github followers]: https://img.shields.io/github/followers/jonnitto.svg?style=social&label=Follow
[follow jon on twitter]: https://img.shields.io/twitter/follow/jonnitto.svg?style=social&label=Follow
[twitter]: https://twitter.com/jonnitto
[fork]: https://github.com/jonnitto/Jonnitto.PrettyEmbedVideoStreaming/fork
[stargazers]: https://github.com/jonnitto/Jonnitto.PrettyEmbedVideoStreaming/stargazers
[subscription]: https://github.com/jonnitto/Jonnitto.PrettyEmbedVideoStreaming/subscription
[followers]: https://github.com/jonnitto/followers
[neos cms]: https://www.neos.io
