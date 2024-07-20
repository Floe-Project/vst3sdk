We use this repository to easily access and maintain the version of the VST3 SDK that we want to use for Floe.

We do this for the following reasons (as of July 2024):
- There is no easy way to download a specific version of the VST3 SDK. There's either url's for the latest version, or a git repo with submodules that needs to be cloned recursively.
- The VST3 SDK includes large amounts of code that we don't want: VSTGUI, tutorials, docs.
- The separate submodules that make up the VST3 SDK give the impression that they are detached and usable separately, but this is not often the case. Each submodule references other submodules assuming they are all accessible from the same root folder. This adds a complication when trying to consume the submodules separately because they must be arranged in the correct folder structure.

Licensed under GPLv3 - see the LICENSE info of the subfolders for further information.
