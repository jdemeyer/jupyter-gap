# jupyter-gap
Jupyter kernels for GAP 

Please note that this software is still in the early stages of development, though should be reasonably usable.

The `wrapper-kernel` is a Jupyter kernel based on the [bash wrapper kernel](https://github.com/takluyver/bash_kernel),
to install

```shell
    python setup.py install
```

To use it, use one of the following:

```shell
    jupyter notebook
    jupyter qtconsole --kernel gap
    jupyter console --kernel gap
```

Note that this kernel requires you to set the environment variable `JUPYTER_GAP_EXECUTABLE` to a valid gap executable or `gap.sh` script, it also depends on the packages [json](https://github.com/gap-packages/json) and [io](https://github.com/gap-packages/io) in recent versions.

If you want to use the `JUPYTER_DotSplash` function, you will need `graphviz` installed and in the path. If you want to use `JUPYTER_TikZSplash`, you will need a `TeX` installation including the `TikZ` packages with `pdflatex` and and `pdf2svg` installed.
