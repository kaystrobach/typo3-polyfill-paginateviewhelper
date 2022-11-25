<!-- PROJECT SHIELDS -->
<!--
*** I'm using markdown "reference style" links for readability.
*** Reference links are enclosed in brackets [ ] instead of parentheses ( ).
*** See the bottom of this document for the declaration of the reference variables
*** for contributors-url, forks-url, etc. This is an optional, concise syntax you may use.
*** https://www.markdownguide.org/basic-syntax/#reference-style-links
-->
[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Issues][issues-shield]][issues-url]
[![GPL License][license-shield]][license-url]


<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#roadmap">Roadmap</a></li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="#acknowledgments">Acknowledgments</a></li>
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
## About The Project

The projects provides a polyfill for the paginateViewHelper widget, which was deprecated in TYPO3 v10 and finally removed in TYPO3 v11+.

* https://docs.typo3.org/other/typo3/view-helper-reference/10.4/en-us/typo3/fluid/latest/Widget/Paginate.html

```html
<f:widget.paginate objects="{blogs}" as="paginatedBlogs" configuration="{itemsPerPage: 5, insertAbove: 1, insertBelow: 0, maximumNumberOfLinks: 10}">
    use {paginatedBlogs} as you used {blogs} before, most certainly inside
    a <f:for> loop.
</f:widget.paginate>
```

One nive thing about the viewHelper was, that it supports pagination up till the database level:

> In the above examples, it looks like {blogs} contains all Blog objects, thus you might wonder if all objects were
> fetched from the database. However, the blogs are NOT fetched from the database until you actually use them, so the
> paginate ViewHelper will adjust the query sent to the database and receive only the small subset of objects.
> So, there is no negative performance overhead in using the Paginate Widget.

### Built With


* PHP
* TYPO3

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- GETTING STARTED -->
## Getting Started

### Prerequisites

You need a project with a supported TYPO3 Version.
Currently this is only TYPO3 Version 11.

### Installation

```bash
composer require kaystrobach/typo3-polyfill-paginateviewhelper
```

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- USAGE EXAMPLES -->
## Usage

```html
<f:widget.paginate objects="{blogs}" as="paginatedBlogs">
   use {paginatedBlogs} as you used {blogs} before, most certainly inside
   a <f:for> loop.
</f:widget.paginate>
```

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- ROADMAP -->
## Roadmap

Don't use this polyfill to jumpstart new projects.
If you are starting a new project follow the Coding guidelines of TYPO3 and use propert current techniques.

* https://docs.typo3.org/m/typo3/reference-coreapi/main/en-us/ApiOverview/Pagination/Index.html

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- CONTRIBUTING -->
## Contributing

Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".
Don't forget to give the project a star! Thanks again!

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

Attention, we will only accept contributions to enhance stability, any changes which modify the behaviour (seen from the fluid side) will be rejected.

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- LICENSE -->
## License

Distributed under the GPL-2.0-or-later License, as this is a derived work from the TYPO3 core. See `LICENSE.txt` for more information.

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- CONTACT -->
## Contact

Kay Strobach - [@kaystrobach](https://twitter.com/kaystrobach)

Project Link: [https://github.com/kaystrobach/typo3-polyfill-paginateviewhelper](https://github.com/kaystrobach/typo3-polyfill-paginateviewhelper)

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- ACKNOWLEDGMENTS -->
## Acknowledgments

Use this space to list resources you find helpful and would like to give credit to. I've included a few of my favorites to kick things off!

* [Choose an Open Source License](https://choosealicense.com)
* [GitHub Emoji Cheat Sheet](https://www.webpagefx.com/tools/emoji-cheat-sheet)
* [Malven's Flexbox Cheatsheet](https://flexbox.malven.co/)
* [Malven's Grid Cheatsheet](https://grid.malven.co/)
* [Img Shields](https://shields.io)
* [GitHub Pages](https://pages.github.com)
* [Font Awesome](https://fontawesome.com)
* [React Icons](https://react-icons.github.io/react-icons/search)

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/kaystrobach/typo3-polyfill-paginateviewhelper.svg?style=for-the-badge
[contributors-url]: https://github.com/kaystrobach/typo3-polyfill-paginateviewhelper/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/kaystrobach/typo3-polyfill-paginateviewhelper.svg?style=for-the-badge
[forks-url]: https://github.com/kaystrobach/typo3-polyfill-paginateviewhelper/network/members
[issues-shield]: https://img.shields.io/github/issues/kaystrobach/typo3-polyfill-paginateviewhelper.svg?style=for-the-badge
[issues-url]: https://github.com/kaystrobach/typo3-polyfill-paginateviewhelper/issues
[license-shield]: https://img.shields.io/github/license/kaystrobach/typo3-polyfill-paginateviewhelper.svg?style=for-the-badge
[license-url]: https://github.com/kaystrobach/typo3-polyfill-paginateviewhelper/blob/master/LICENSE.txt
