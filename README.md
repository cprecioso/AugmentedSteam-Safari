# AugmentedSteam-Safari

Very preliminary Safari wrapper for the [original Augmented Steam extension](https://github.com/tfedor/AugmentedSteam).

Starting off from the default Safari Web Extension template in Xcode, I made the [`Resources` folder](./AugmentedSteam-Safari/AugmentedSteam-Safari Extension/) a submodule pointing to the extension code.
I then added two build phases in Xcode, one for copying all the files from `Resources` into the extension, and another one to copy `manifest.json` inside as well. [`manifest.json` is sym-linked to `manifest-chrome.json` inside the submodule.](./AugmentedSteam-Safari/AugmentedSteam-Safari Extension/manifest.json)
