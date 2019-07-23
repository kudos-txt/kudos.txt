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

**Kudos** (from the Ancient Greek: κῦδος) is acclaim or praise for exceptional
achievement.

### What is kudos.txt

kudos.txt provides a format to express gratitude to your contributors. It is
easy to understand, easy to read for humans and machines and it does not force
you to present data, that you don't want to present. You can extend it or reduce
it to your needs.

### Why a text file

A text file is easy to read from humans and machines. It is portable and can
be used in any OS. It does not require a graphical desktop and can be read and
manipulated even without a text editor.

### Differences to humans.txt

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

### Syntax

Kudos.txt is heavily inspired by YAML. You will find the following parts in
the example kudos.txt:

```
# The (<...>) are indicating, that you should replace them with your string.

# A leading hash (#) indicates a comment.
# <comment>

# A section has no indention.
<section>:
# Each section contains of list items (-), which can have multiple items and
# values assigned.
  - <item1>: <value1>
    <item2>: <value2>

  - <item3>: <value3>
    <item4>: <value4>
```

### Section

> Definition: a word, which indicates a context

The `<section>:` is indicating a context switch. For now, the below sections are
defined and standardized. You can add more, if you feel the need. Please also
feel free to open an issue.

1.  **project**

    This section consists of information about the project.

2.  **contributor**

    A section containing a list of your contributors with some optional
    information.

3.  **partner**

    A section containing a list of your partners, if you have some and want to
    mention them.

4.  **software**

    A section containing a list of used software or libraries in your project.

### Item

> Definition: a 4-letter word, which indicates a specific type of information

Items are indicators for a specific information. You can use them optionally in
any section. The example [kudos.txt](./src/kudos.txt) is giving an idea, what
makes sense. You can add new items, if you feel the need. The standardized items
are:

1.  **name**

    The real name, nick or any other presentation of "who".

1.  **site**

    A website url like "https://example.com". You can specify multiple urls
    separated by commas.

1.  **blog**

    A blog url like "https://blog.example.com".

1.  **help**

    A support url like "https://help.example.com" or
    a support contact like "help@example.com" or
    a support contact number like "+49 111 222 333".

1.  **news**

    A support url to your newsfeed or newsletter or any other source of news.

1.  **mail**

    A mail address to contact the **name** like "name@example.com"

1.  **chat**

    A chat address in the form of "skype:mynick" to present your nick or
    "slack:mychannel" to indicate a channel or
    "https://chat.example.com" to indicate a url to your chat information.

1.  **home**

    An indicator of your home. You can use as many information as you want
    separated by commas.

1.  **work**

    An indicator to show your workplace. This can be the company name or
    job title or job description or something abstract.

1.  **note**

    A field, where you can put any other note down.

### Example

Names derived from [Alice and Bob](https://en.wikipedia.org/wiki/Alice_and_Bob)

**Simple Example**

If you want to list the contributors, this example may be a good start.

```
project:
  - name: Alice and Bob - The Movie
    site: https://example.com

contributor:
  - name: Alice
    role: Main Character
  - name: Bob
  - name: Carol
  - name: Chuck
    role: Bad guy
```

**Advanced Example**

You can also put empty lines between each item, for better readability and
provide addional information

```
project:
  - name: Alice and Bob - The Movie
    site: https://example.com
    mail: mail@example.com

contributor:
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

partner:
  - name: example.org
    site: https://example.org
    note: Very useful for examples.

software:
  - name: VIM
    note: Any other editor may work, too.
```

## FAQ

1.  **Q** Do I need to put information 'xxx' in my kudos.txt?

    **A** No, you can reduce the amount of information, if you want.

2.  **Q** Why are 4-letter / 4-character items enforced?

    **A** This allows a very clear readability for many humans.

3.  **Q** I want to have a section "developers" and "managers". Is this possible?

    **A** Yes, you can add sections, if you want. Please also feel free to contribute.

4.  **Q** Do you offer any tools to parse the kudos.txt in [html|markdown|json|x]?

    **A** Not yet, but this is definitively the plan. Please feel free to help.

5.  **Q** Why do you came up tith kudos.txt?

    **A** We wanted to establish something standardized, machine and human
    readable to express gratitude to contributors, partners, etc.

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
