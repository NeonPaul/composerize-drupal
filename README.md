# Composerize Drupal - D7 hack

This is a proof-of-concept hack on [composerize-drupal](https://github.com/grasmash/composerize-drupal) to get it working with D7 projects.

To get it working, you first have to add a minimum composer.json file to your project, as per [https://github.com/drush-ops/drush-launcher/issues/33#issuecomment-380095772](https://github.com/drush-ops/drush-launcher/issues/33#issuecomment-380095772)

```json
{
    "extra": {
        "installer-paths": {
            ".": ["type:drupal-core"]
        }
    }
}
```

Then run the commands as normal.

I probaly won't be maintaining this as it no longer suits my needs (most of the packages on the project I'm maintaining do not have an appropriate composer version and will have to be updated manually), but I'll leave it up for anyone else who might find it useful.
