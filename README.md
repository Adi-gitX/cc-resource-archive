

---

# CC Resource Archive

Welcome to the CC Resource Archive, a collection of resources on Creative Commons (CC) tools and other open topics. This project aims to provide a simple and easy-to-update area for tracking useful resources related to Creative Commons licenses and open content topics. The live site is available at [resources.creativecommons.org](https://resources.creativecommons.org/).

## Overview

### Code of Conduct
Before getting started, please review our [Code of Conduct](https://opensource.creativecommons.org/community/code-of-conduct/) to understand our commitment to fostering a welcoming community. If you encounter any unacceptable behavior, please report it to [conduct@creativecommons.org](mailto:conduct@creativecommons.org).

### Contributing
We welcome contributions! Please see our [Contribution Guidelines](https://github.com/creativecommons/.github/blob/main/CONTRIBUTING.md) for details on how to get involved.

## How it Works
The website is built using [Jekyll](http://jekyllrb.com/docs/home/), a simple templating system integrated with GitHub. All site pages are located in the `docs/` directory. This README file and the resource template are in the main branch.

To submit a resource, make a copy of the [Resource Template](https://github.com/creativecommons/cc-resource-archive/blob/main/resourcetemplate.md), fill in the fields accordingly, and create a new file with the appropriate format (.html, .md, or .textile).

## Category URLs
You can filter resources using URLs. For example, to view videos available in English about licenses, use:
- [View English License Videos](http://resources.creativecommons.org/all/?&topic=licenses&medium=video&language=en)

## The Index Page
The index page showcases up to 16 featured items. Each featured page has a "featured" variable indicating the order of appearance.

## Menu Categories
The homepage menu categories are defined in `.yml` files in the `_data/` folder. Use the `name` and `string` values for topics, media, and languages.

## Local Development

### Docker Compose Setup

1. **Install Docker Engine:**
   - [Docker Engine Installation Instructions](https://docs.docker.com/engine/install/)

2. **Clone the Repository:**
   ```shell
   git clone https://github.com/creativecommons/cc-resource-archive.git
   cd cc-resource-archive
   ```

3. **Run the Container:**
   ```shell
   docker compose up
   ```
   - This will build the container if it's the first time.
   - Access the site at [localhost:4000](http://localhost:4000/)

4. **Stop the Container:**
   ```shell
   docker compose down
   ```
   - To stop the app from running, simply open another instance of the terminal and type `docker compose down`.
   - Alternatively, you can revisit the existing terminal running the container and type `CTRL + C`.

## Screenshots

Here are some screenshots of the CC Resource Archive:

1. **Homepage:**
   ![Homepage](path/to/homepage-screenshot.png)

2. **Resource Page:**
   ![Resource Page](path/to/resource-page-screenshot.png)

## License

### Code
The code in this repository is licensed under the [Expat/MIT License](LICENSE).

### Content/Text
[![CC BY 4.0 license button](https://licensebuttons.net/l/by/4.0/88x31.png#floatleft)](https://creativecommons.org/licenses/by/4.0/)

All content is licensed under a [Creative Commons Attribution 4.0 International License](https://creativecommons.org/licenses/by/4.0/) unless otherwise specified.

Feel free to reach out with any questions or suggestions. Thank you for contributing to the CC Resource Archive!

---

