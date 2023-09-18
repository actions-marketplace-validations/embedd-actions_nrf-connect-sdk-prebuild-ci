# nrf-connect-sdk-ci
Build NRF Connect SDK projects

This action uses an prebuild image by dockerfile from the repository: https://github.com/embedd-actions/nrf-connect-sdk-ci 

## Usage example:

```
jobs:
  build:

    runs-on: ubuntu-latest

    steps:
    - uses: actions/checkout@v3


    - name: Build
      uses: embedd-actions/nrf-connect-sdk-prebuild-ci@v2.3.0
      with:
        board: nrf52833dk_nrf52833
        build_dir: build

```
