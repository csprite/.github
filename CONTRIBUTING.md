# Contributing

if you are a developer and want to contribute to the csprite codebase read more about following before contributing:
- [Code Style, Structure & Contribution Guidelines](#code-style-structure--contribution-guidelines)
- [The Contributor License Agreement](https://github.com/csprite/.github/blob/master/CLA.md)

## Code Style, Structure & Contribution Guidelines

- **Please understand that by submitting a PR you are also submitting a request for the maintainer to review your code and then take over its maintenance.** PR should be crafted both in the interest of the end-users and also to ease the maintainer into understanding and accepting it. 
- Many PRs are useful to demonstrate a need and a possible solution but aren't adequate for merging (causing other issues, not seeing other aspects of the big picture, etc.). In doubt, don't hesitate to push a PR because that is always the first step toward finding the mergeable solution! Even if a PR stays unmerged for a long time, its presence can be useful for other users and helps toward finding a general solution.
- **Make sure you create a branch dedicated to the pull request**. In Git, 1 PR is associated to 1 branch. If you keep pushing to the same branch after you submitted the PR, your new commits will appear in the PR.
- **When adding a feature,** please describe the usage context (how you intend to use it, why you need it, etc.). Be mindful of [The XY Problem](http://xyproblem.info/). 
- **When fixing a warning or compilation problem,** please post the compiler log and specify the compiler version and platform you are using.
- **Attach screenshots (or GIF/video) to clarify the context and demonstrate the feature at a glance.** You can drag pictures/files in the message edit box. Prefer the long-term longevity of GitHub attachments over 3rd party hosting (you can drag pictures into your post).
- **Follow [KISS Principle](https://en.wikipedia.org/wiki/KISS_principle)**: make sure your contribution **K**eeps **I**t **S**imple **S**tupid, the more simple the codebase the more it's easy for everyone to understand, if you are writing too many comments then it's time to re-think cause it's probably not simple but stupid.
- **Make sure your code follows the coding style already used in the codebase:**
  - Tab indentations (no spaces if possible)
  - Local variable names: `local_variable`/`localVariable`
  - 'Global' function names: `FunctionName()`
  - 'Local' function names: `_functionName()`/`functionName()`
  - Comments: `// Text Comment` / `//CodeComment();`
  - Casts: C-style casts in most cases if possible
- **Make sure your directory/file structure is:**
  - `.cpp`, `.c` files contain implementation of a particular feature, like a `config.cpp` would contain functions for working with config files.
  - `.hpp`, `.h` files contain the publicly available function available by that corresponding `.cpp` / `.c` file.
  - if there are more than 2 files for a particular implementation it should be transferred into it's own directory.
