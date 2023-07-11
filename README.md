[![License](https://img.shields.io/badge/License-Apache%202-blue.svg)](LICENSE)

# The acados_nav2_plugins repository
A collection of acados-based plugins for [Navigation2](https://navigation.ros.org/). In detail, this repository contains two ROS 2 packages:

*   [acados_nav2_export](acados_nav2_export/) provides a library to export [acados](https://docs.acados.org/)-based solvers for use in Navigation2.
*   [acados_nav2_controller](acados_nav2_controller/) provides controller plugins for Navigation2.

Technical information on the interfaces and use of these packages is given in the README.md files in the corresponding subfolders.

## NOTICE

This repository is currently (date of writing: July 11, 2023) still under construction. Primarily finishing preparations in dependency repositories:
* [boschresearch/blasfeo-vendor](https://github.com/boschresearch/blasfeo-vendor)
* [boschresearch/hpipm-vendor](https://github.com/boschresearch/hpipm-vendor)
* [boschresearch/acados](https://github.com/boschresearch/acados)
Please check back later this week for updates...


## Purpose of the project

The software is not ready for production use. It has neither been developed nor tested for a specific use case. However, the license conditions of the applicable Open Source licenses allow you to adapt the software to your needs. Before using it in a safety relevant setting, make sure that the software fulfills your requirements and adjust it according to any applicable safety standards (e.g. ISO 26262).


## Requirements, how to build, test, install, use, etc.

Clone the repository into a ROS workspace and build it using [colcon](https://colcon.readthedocs.io/).


## License

acados_nav2_plugins is open-sourced under the Apache-2.0 license. See the [LICENSE](LICENSE) file for details.

For a list of other open source components included in acados_nav2_plugins, see the file [3rd-party-licenses.txt](3rd-party-licenses.txt).


## Quality assurance

The colcon_test tool is used for quality assurances, which includes cpplint, uncrustify, flake8, xmllint and various other tools.


## Known issues/limitations

Please notice the following issues/limitations:

*   Currently, not all QP solvers ar supported. Only HPIPM QP solver can be selected.

