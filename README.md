Sure! Here's an updated and formatted version of the README with additional installation steps:

---

# CC Resource Archive

Collection of resources on Creative Commons (CC) tools and other open topics

## Overview

Welcome to the CC Resources Archive. The idea of this project is to have a simple, easy-to-update area for keeping track of all of the useful resources that people make about Creative Commons licenses and open content topics in general. The live site is at [resources.creativecommons.org](https://resources.creativecommons.org/).

## Code of Conduct

[`CODE_OF_CONDUCT.md`](https://github.com/creativecommons/.github/blob/main/CODE_OF_CONDUCT.md):
> The Creative Commons team is committed to fostering a welcoming community. This project and all other Creative Commons open source projects are governed by our [Code of Conduct](https://opensource.creativecommons.org/community/code-of-conduct/). Please report unacceptable behavior to [conduct@creativecommons.org](mailto:conduct@creativecommons.org) per our [reporting guidelines](https://opensource.creativecommons.org/community/code-of-conduct/enforcement/).

## Contributing

See [`CONTRIBUTING.md`](https://github.com/creativecommons/.github/blob/main/CONTRIBUTING.md).

## How it works

The website is built using [Jekyll](http://jekyllrb.com/docs/home/), a simple templating system that's built into GitHub. All of the site pages are in the `docs/` directory. This README file and the resource template are in the main branch.

To submit a resource, make a copy of [`resourcetemplate.md`](https://github.com/creativecommons/cc-resource-archive/blob/main/resourcetemplate.md) and change the values for each field accordingly. The space below the front matter is freeform, for providing additional information or links. The resource template also includes explanations of each of the fields.

### Category URLs

You can format the `resources.creativecommons.org/all?` URL to show any category or combination of categories you want. For example, videos available in English about licenses:

- [View English License Videos](http://resources.creativecommons.org/all/?&topic=licenses&medium=video&language=en)

You can use any category that's listed in one or more resources pages, not just the ones available in the menu on "all." For example, resources about music:

- [Resources about Music](http://resources.creativecommons.org/all/?&topic=music)

### The index page

The index page pulls up to 16 featured items. Each featured page has a "featured" variable. The number is the order in which they should appear.

### Menu categories

The list of topics, media, and languages on the homepage is dictated by the three respective `.yml` files in the `_data/` folder. For each category, we provide a capitalized name and a lowercase string with no punctuation. For example:

- name: Licenses
  string: licenses

- name: Public Domain
  string: publicdomain

- name: Open Educational Resources
  string: oer

The reason for setting it up this way is that the "string" value is what's used in the URLs and CSS classes. It's also what you use in the resource page itself to identify the category. So these should be relatively short, but still sensical.

## Local Development

### Docker Compose setup

1. **Install Docker Engine:**
   - [Docker Engine Installation Instructions](https://docs.docker.com/engine/install/)

2. **Clone the Repository:**
   ```shell
   git clone https://github.com/creativecommons/cc-resource-archive.git
   cd cc-resource-archive
   ```

3. **Run the container:**
   ```shell
   docker compose up
   ```
   - This will build the container if it's the first time.
   - The docker container may take some time to start. When it's ready, you should see:
     ```
     jekyll-cc-resource-archive  |     Server address: http://0.0.0.0:4000
     jekyll-cc-resource-archive  |   Server running... press ctrl-c to stop.
     ```
   - Once running successfully, you can access the site in your browser at [localhost:4000](http://localhost:4000/)

4. **Stop the container:**
   - To stop the app from running, simply open another instance of the terminal and type:
     ```shell
     docker compose down
     ```
   - Alternatively, you can revisit the existing terminal running the container and type `CTRL + C`

## Screenshots

Here are some screenshots of the CC Resource Archive:

- Homepage: ![Homepage](path/to/homepage-screenshot.png)
- Resource Page: ![Resource Page](path/to/resource-page-screenshot.png)

## License

### Code

The code in this repository is licensed under the [Expat/MIT License](LICENSE).

### Content/Text

[![CC BY 4.0 license button](https://licensebuttons.net/l/by/4.0/88x31.png#floatleft)](https://creativecommons.org/licenses/by/4.0/)

All content is licensed under a [Creative Commons Attribution 4.0 International License](https://creativecommons.org/licenses/by/4.0/) unless otherwise specified.

Feel free to reach out with any questions or suggestions. Thank you for contributing to the CC Resource Archive!

---

Please replace `path/to/homepage-screenshot.png` and `path/to/resource-page-screenshot.png` with the actual paths to your screenshots.

All the content within this repository is licensed under a [Creative Commons
Attribution 4.0 International License][cc-by] unless otherwise specified.

[cc-by-png]: https://licensebuttons.net/l/by/4.0/88x31.png#floatleft "CC BY 4.0 license button"
[cc-by]: https://creativecommons.org/licenses/by/4.0/ "Creative Commons Attribution 4.0 International License"
