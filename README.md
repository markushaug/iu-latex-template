# LaTeX template for academic papers at IU International University

This repository contains a LaTeX template for academic papers at [IU International University](https://www.iu.de/). The template is tailored to the requirements of IU International University and takes into account all formalities known to me that apply to the submission of academic papers at IU International University.

## Disclaimer

This template is provided without guarantee or warranty. The author assumes no responsibility for the accuracy or reliability of the information contained in this template or for the consequences of its use. Please use it at your own risk and responsibility.

## Usage

To use this template, simply clone or download this repository and start writing your scientific paper. Please make sure you keep the original credits in the source code. Don't worry, this will not be visible in any of your submissions :).

Please note that the use of LuaHBTeX, version 1.15.0 (TeX Live 2022) is required. If you use Overleaf, you can easily change this in the settings of the respective work, locally you have to configure it accordingly.

Alternatively, you can open the repository in Visual Studio Code and use the LaTeX Workshop Extension to generate the PDF. A devcontainer automatically downloads and installs the required TeX Live version. All other required packages are also installed automatically.

### Commands

To generate the PDF, execute the following command:

```shell
$ lualatex main
```

In case of changes to the `.bib` file, the following command must be executed to update the references:

```shell
$ biber main
```

## Licence

This template is licensed under the MIT Licence. See the [LICENSE](LICENSE) file for more information.
