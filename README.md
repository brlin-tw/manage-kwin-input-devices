# manage-kwin-input-devices

A utility to manage the disable/enable state of input devices under Kwin(works under KDE Wayland).

<https://gitlab.com/brlin/manage-kwin-input-devices>  
[![The GitLab CI pipeline status badge of the project's `main` branch](https://gitlab.com/brlin/manage-kwin-input-devices/badges/main/pipeline.svg?ignore_skipped=true "Click here to check out the comprehensive status of the GitLab CI pipelines")](https://gitlab.com/brlin/manage-kwin-input-devices/-/pipelines) [![GitHub Actions workflow status badge](https://github.com/brlin-tw/manage-kwin-input-devices/actions/workflows/check-potential-problems.yml/badge.svg "GitHub Actions workflow status")](https://github.com/brlin-tw/manage-kwin-input-devices/actions/workflows/check-potential-problems.yml) [![pre-commit enabled badge](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white "This project uses pre-commit to check potential problems")](https://pre-commit.com/) [![REUSE Specification compliance badge](https://api.reuse.software/badge/gitlab.com/brlin/manage-kwin-input-devices "This project complies to the REUSE specification to decrease software licensing costs")](https://api.reuse.software/info/gitlab.com/brlin/manage-kwin-input-devices)

\#kwin \#kde \#wayland \#device-management \#linux

## Usage

Refer to the following instructions to use this utility:

1. Acquire the release archive from [the Releases page](https://gitlab.com/brlin/manage-kwin-input-devices/-/releases).
1. Extract the release archive using an archive manipulation program.
1. Launch a text terminal.
1. In the text terminal, run the following command to use the utility:

    ```bash
    /path/to/manage-kwin-input-devices-X.Y.Z/manage-kwin-input-devices _operation_mode_ _arguments_...
    ```

   Replace the `/path/to/manage-kwin-input-devices-X.Y.Z/manage-kwin-input-devices`, the `_operation_mode_` and the `_arguments_` placeholder text to their respective values.  Refer to [the manual page](manage-kwin-input-devices.1.md) for more information.

## Credits

This project is based on [Amine Hassane](https://gist.github.com/Sporif)'s work: [Enable or disable input devices on KDE](https://gist.github.com/Sporif/0e52e4b0eaf071cfbf19f3381ba3d65a).

## Licensing

Unless otherwise noted([comment headers](https://reuse.software/spec-3.3/#comment-headers)/[REUSE.toml](https://reuse.software/spec-3.3/#reusetoml)), this product is licensed under [The MIT License](https://opensource.org/license/mit).

This work complies to [the REUSE Specification](https://reuse.software/spec/), refer to the [REUSE - Make licensing easy for everyone](https://reuse.software/) website for info regarding the licensing of this product.
