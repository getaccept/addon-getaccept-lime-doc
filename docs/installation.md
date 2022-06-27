hero: Close your Lime CRM deals faster with GetAccept

# Installation Instructions

## Preparations

1. Check that the requirements are met.

## Installation

1. In the file `pyproject.toml` in the code repository of the Lime CRM solution, under the section `[tool.poetry.dependencies]`, add the following text on a separate line: `getaccept = '==<version>'`, where `<version>` is replaced with the actual version of this add-on that you are installing. Use the latest one described in the [Changelog](changelog.md). For example: `getaccept = '== 1.0.20'`.
2. Build the Lime CRM solution as normally done, and install it as normally done.
3. In Lime Admin, in the card view configuration for Deal, Company and Person, add the following web component: `lwc-getaccept-root`.
