# age-rs [![Bors enabled](https://bors.tech/images/badge_small.svg)](https://app.bors.tech/repositories/24826)

##### Cross-platform RTS game engine based on Age of Empires mechanics

For now we focus to port [`nyan`](https://github.com/SFTtech/nyan) and [`libopenage` (part of openage)](https://github.com/SFTtech/openage/tree/master/libopenage) 
to [rust-lang](https://www.rust-lang.org/) and create a stable toolchain around it. Both are part of the engine core of [openage](https://github.com/SFTtech/openage/) which is
written mainly in **C++17** and **Python 3**. While we are trying to stick to fundamental design decisions (regarding e.g. architecture, multiplayer) that 
the openage authors did - we are going to use Rust to build a reliable cross-platform toolchain that empowers everyone to develop on **age-rs**
easily and efficiently.

Goals
-----

* reimplement `nyan`
* reimplement `libopenage`
* create a stable `rust/python-interface`
* create extensive documentation around the project


* Ultimate goals: 
    * lower the bar on developing
    * create secure, reliable software that is easy to maintain long-term


Current State of the Project
----------------------------

This project has just begun, if you are eager to help feel free to contribute or open an issue to get in touch.
You can also send me a message on Discord: `simonsanone#4039`

Cloning this repository
-----------------------

As we are dealing with git submodules here, you should use the following command to clone, initialize and update:

`git clone --recurse-submodules https://github.com/age-rs/age-rs.git`

If you need more information you find them here in the [Git submodules documentation](https://web.archive.org/web/20200508192857/https://git-scm.com/book/en/v2/Git-Tools-Submodules)

How to contribute?
------------------

If you want to contribute to this project feel free to do so. The easiest way would be that you fork this repository, 
create a branch for the things you want to do and make a PR to this main repository.

We've collected some essential knowledge about contributions in [contributing](doc/contributing.md), please read it.


Dependencies, Building and Running
----------------------------------

- You will need everything that is stated in the [openage build documentation](https://github.com/simonsan/openage/blob/master/doc/building.md)
    - so you will need to be able to build openage it self for the beginning
    - if you have any questions, feel free to ask either the openage-authors or send me a message on Discord (`simonsanone#4039`) 
    - you can also ask in the [forum of openage](https://forum.openage.dev) for help (I'm active there as well)

- Make sure you initialize and use the submodules of `nyan` and `openage` from this repository here as we will probably need to patch
some things in/out for compatibility reasons

License
-------

**GNU GPLv3** or later; see [COPYING.md](COPYING.md) and [LICENSE](LICENSE).

I know that probably nobody is ever gonna look at the `COPYING` file,
but if you want to contribute code to openage, please take the time to
skim through it and add yourself to the authors list.
