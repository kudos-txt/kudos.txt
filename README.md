<!--
name: README.md
description: This file contains important information for the repository.
author: kudos-txt.io
contact: hello@kudos-txt.io
license: BSD-3-Clause
-->

<!-- github shields -->
[![Github (tag)](https://img.shields.io/github/tag/kudos-txt/kudos.txt.svg)](https://github.com/kudos-txt/kudos.txt/tags)
[![Github (license)](https://img.shields.io/github/license/kudos-txt/kudos.txt.svg)](https://github.com/kudos-txt/kudos.txt/blob/master/LICENSE)
[![Github (issues)](https://img.shields.io/github/issues/kudos-txt/kudos.txt.svg)](https://github.com/kudos-txt/kudos.txt/issues)
[![Github (pull requests)](https://img.shields.io/github/issues-pr/kudos-txt/kudos.txt.svg)](https://github.com/kudos-txt/kudos.txt/pulls)

# kudos.txt

Express gratitude to your contributors.

## Motivation

Thousands of Open Source Repositories are hosting code. But we should never
forget, that this code is made by people. Are these people getting the gratitude
they deserve? We think, it is time to have a kudos.txt to express the gratitude
to all of the contributors and give them a place outside of git logs.

## Description

Kudos (from the Ancient Greek: κῦδος) is acclaim or praise for exceptional
achievement.

### What is kudos.txt

kudos.txt provides a format to express gratitude to your contributors. It is
easy to understand, easy to read for humans and machines and it does not force
you to present data, that you don't want to present.

### Why a textfile

A textfile is easy to read from humans and machines. It is portable and can
be used in any OS. It does not require a graphical desktop or even a text editor.

### Difference to humans.txt

[humans.txt](humanstxt.org) is a very nice approach. In fact, it even inspired
the creators of kudos.txt. Nevertheless, the approach is different.

-   humans.txt focusses on websites, kudos.txt can be used for any contribution.
-   humans.txt is not easy to be read from machines / software, kudos.txt uses
    yaml syntax.
-   humans.txt uses indicators of different length, kudos enforces 4-character
    indicators.
-   humans.txt differentiates between team and outside collaborators, kudos.txt
    does not. Everybody should be seen as a contributor, when interacting with
    a project.

## Requirements

A Text Editor is helpful.

## Installation

No installation is needed. Just download the [kudos.txt](./src/kudos.txt).

## Usage

Copy the [kudos.txt](./src/kudos.txt) to your repository and fill in your data.

### Sections

Currently 4 sections are standardized. You are free to use them or not.

1.  project
    Contains information for the project itself.
2.  contributors
    Contains the contributor information to kudos the contributors.
3.  partners
    This section should contain partner projects, sponsors or otherwise related
    teams, companies or products.
4.  software
    Some projects are using libraries or software from other projects.
    These can be mentioned here, to kudos them.

### Items

Items are listed in the sections.

Each item contains 2 types of information.

1.  mandatory
    If you want to add an item to a section, you only need to fill the `- name:`.
    You can use your real name or project handle/nick.
2.  optional
    All other information are optional and can be filled in. Nobody should be
    forced to fill in his `mail` or `site`.

### Syntax

The syntax is heavily inspired by [YAML](https://yaml.org). This will allow
to use a YAML Linter or any other YAML Tool to process the file. It is also
very easy to be read from humans.

### Example

Names derived from [Alice and Bob](https://en.wikipedia.org/wiki/Alice_and_Bob)

**Simple Example**

If you want to list the contributors, this may be a good idea.

```
contributors:
  - name: Alice
    role: Main Character
  - name: Bob
  - name: Carol
  - name: Chuck
    role: Bad guy
```

**Advanced Example**

You can also put an empty line between each item, for better readability.

```
project:
  - name: Alice and Bob - The Movie
    site: example.com

contributors:
  - name: Alice
    role: Main Character
    mail: alice@example.com
    home: Not in wonderland

  - name: Bob
    role: Main Character
    mail: bob@example.com
    note: Bob sends many mails.

  - name: Chuck
    role: Bad Guy
    mail: secret@spam.example.com
    work: room 404

partners:
  - name: example.com
    site: example.com
    note: Very useful for examples.

software:
  - name: Mail Client
```

## Contribute

Thank you so much for considering to contribute. We are very happy, when somebody
is joining the hard work. Please fell free to open
[Bugs, Feature Requests](https://github.com/kudos-txt/kudos.txt/issues)
or [Pull Requests](https://github.com/kudos-txt/kudos.txt/pulls) after
reading the [Contribution Guideline](https://github.com/while-true-do/doc-library/blob/master/docs/CONTRIBUTING.md).

See who has contributed already in the [kudos.txt](./kudos.txt).

## License

This work is licensed under a [BSD-3-Clause License](https://opensource.org/licenses/BSD-3-Clause).

## Contact

-   Site <https://kudos-txt.io>
-   Twitter <https://twitter.com/wtd_news>
-   Code <https://github.com/kudos-txt>
-   Mail [hello@kudos-txt.io](mailto:hello@kudos-txt.io)
-   IRC [freenode, #while-true-do](https://webchat.freenode.net/?channels=while-true-do)
-   Telegram <https://t.me/while_true_do>
