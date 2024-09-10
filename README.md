![](../../workflows/gds/badge.svg) ![](../../workflows/docs/badge.svg) ![](../../workflows/test/badge.svg) ![](../../workflows/fpga/badge.svg)

# Tiny Tapeout Silice Project Template

- [Read the documentation for project](docs/info.md)

## What is Tiny Tapeout?

Tiny Tapeout is an educational project that aims to make it easier and cheaper than ever to get your digital and analog designs manufactured on a real chip.

To learn more and get started, visit https://tinytapeout.com.

## What is Silice?

[Silice](https://github.com/sylefeb/Silice/) is an easy-to-learn, powerful hardware description language, that simplifies designing hardware algorithms with parallelism and pipelines. This project template provides a simple VGA output framework example for Tiny Tapeout, see [source here](src/silice/vga_demo.si).

## Set up your Silice project

1. Edit and add silice files into the `src/silice` folder.
2. Edit the [info.yaml](info.yaml) and update information about your project, paying special attention to the `top_module` properties. You have to choose a new name for the top module, replacing `tt_um_projectname` by a different name starting with `tt_um_`. The name has to be updated in different locations:
   - [info.yaml](info.yaml)
   - Silice [Makefile](src/silice/Makefile)
   - test bench [tb.v](test/tb.v)

> If these names are not properly updated and/or the info.md file mandatory information is not specified, the github automated actions will report errors.

3. Edit [docs/info.md](docs/info.md) and add a description of your project.
4. Adapt the testbench to your design. See [test/README.md](test/README.md) for more information.

The GitHub action will automatically build the ASIC files using [OpenLane](https://www.zerotoasiccourse.com/terminology/openlane/).

## Enable GitHub actions to build the results page

- [Enabling GitHub Pages](https://tinytapeout.com/faq/#my-github-action-is-failing-on-the-pages-part)

## Resources

- [FAQ](https://tinytapeout.com/faq/)
- [Digital design lessons](https://tinytapeout.com/digital_design/)
- [Learn how semiconductors work](https://tinytapeout.com/siliwiz/)
- [Join the community](https://tinytapeout.com/discord)
- [Build your design locally](https://www.tinytapeout.com/guides/local-hardening/)

## What next?

- [Submit your design to the next shuttle](https://app.tinytapeout.com/).
- Edit [this README](README.md) and explain your design, how it works, and how to test it.
- Share your project on your social network of choice:
  - LinkedIn [#tinytapeout](https://www.linkedin.com/search/results/content/?keywords=%23tinytapeout) [@TinyTapeout](https://www.linkedin.com/company/100708654/)
  - Mastodon [#tinytapeout](https://chaos.social/tags/tinytapeout) [@matthewvenn](https://chaos.social/@matthewvenn)
  - X (formerly Twitter) [#tinytapeout](https://twitter.com/hashtag/tinytapeout) [@tinytapeout](https://twitter.com/tinytapeout)
