# Contributing

To contribute to this repository, all you need to install is [`uv`](https://docs.astral.sh/uv). Once you have that installed, here are some useful commands you can run:

- Start Jupyter Lab
  ```shell
  uv run jupyter lab docs
  ```
- Build a local version of the Jupyter Lite server:
  ```shell
  uv run \
    --group lite \
    --no-dev \
    jupyter lite build \
      --contents docs/Dp-to-pip-pip-pim.ipynb \
      --contents docs/Dp-to-pip-pip-pim-fixed.ipynb \
      --output-dir lite
  ```
- Run all notebooks
  ```shell
  uv run --group test --no-dev pytest
  ```

For more information about developer tools for ComPWA repositories, see **[compwa.github.io/develop](https://compwa.github.io/develop)**.
