[![Latest stable version]][packagist] [![Total downloads]][packagist] [![License]][packagist] [![GitHub forks]][fork] [![Donate Paypal]][paypal] [![Wishlist amazon]][amazon] [![GitHub stars]][stargazers] [![GitHub watchers]][subscription] [![GitHub followers]][followers] [![Follow Jon on Twitter]][twitter]

# Jonnitto.PrettyEmbedVideoStreaming

Prettier embeds for your native streaming videos in [Neos CMS] - with excellent options like high-res preview images, lightbox feature, captions, and advanced customization of embed options.

## Installation

Most of the time, you have to make small adjustments to a package (e.g., a configuration in `Settings.yaml`). Thus, it is essential to add the corresponding package to the composer from your theme package. Mostly this is the site package located under `Packages/Sites/`. To install it correctly, go to your theme package (e.g.`Packages/Sites/Foo.Bar`) and run the following command:

```bash
composer require jonnitto/prettyembedvideostreamingstreaming --no-update
```

The `--no-update` command prevent the automatic update of the dependencies. After the package was added to your theme `composer.json`, go back to the Neos installation's root and run `composer update`. Et voilà! Your desired package is now installed correctly.

## Customization

### Configuration

If you want to customize the default settings, take a look at the [Settings.Jonnitto.yaml] file. If no node property is giving, these default values will be taken. If you, for example, don't want to let the editor choose if the video should open in a lightbox, you can deactivate the mixin in your Configuration folder like this:

```yaml
"Jonnitto.PrettyEmbedVideoStreaming:Content.Video":
  superTypes:
    "Jonnitto.PrettyEmbedHelper:Mixin.Lightbox": false
```

These are the available mixins used for the video:

| Mixin name (Prefix: `Jonnitto.PrettyEmbedHelper:`) | Description                                                                                                      | Default value | Enabled per default |
| -------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------- | :-----------: | :-----------------: |
| `Mixin.Groups`                                     | Enables the inspector groups                                                                                     |               |          ✓          |
| `Mixin.IncludeAssets`                              | Include the frontend resources                                                                                   |               |          ✓          |
| `Mixin.Image`                                      | Add the preview image property                                                                                   |               |          ✓          |
| `Mixin.Lightbox`                                   | Open the video in a lightbox                                                                                     |    `false`    |          ✓          |
| `Mixin.Title`                                      | Set the title to identify the video in the content tree easily, and pass the title as `aria-label` to the video. |               |          ✓          |
| `Mixin.Loop`                                       | Loop the video                                                                                                   |    `false`    |                     |
| `Mixin.Controls`                                   | Show the controls                                                                                                |    `true`     |                     |
| `Mixin.Autoplay`                                   | Autoplays the video                                                                                              |    `false`    |                     |
| `Mixin.Muted`                                      | Mutes the video                                                                                                  |    `false`    |                     |

### Fusion

If you want to use the player as a pure component, you can use the [`Jonnitto.PrettyEmbedVideoStreaming:Component.Video`] fusion prototype.

If you want to read the node properties and let the package handle all for you, you should use the [`Jonnitto.PrettyEmbedVideoStreaming:Content.Video`] prototype. For easier including in your node types, you can disable the content element wrapping with `contentElement = false`. This is useful if you want to create, for example, a text with a video node type.

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
[license]: LICENSE
[neos cms]: https://www.neos.io
[settings.jonnitto.yaml]: Configuration/Settings.Jonnitto.yaml
[`jonnitto.prettyembedvideostreaming:component.video`]: Resources/Private/Fusion/Component/Video.fusion
[`jonnitto.prettyembedvideostreaming:content.video`]: Resources/Private/Fusion/Content/Video.fusion
