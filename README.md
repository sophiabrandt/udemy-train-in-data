[![Contributors][contributors-shield]][contributors-url]
[![Issues][issues-shield]][issues-url]
[![BSD-3-Clause License][license-shield]][license-url]

<!-- PROJECT LOGO -->
<br />
<p align="center">
  <a href="https://github.com/sophiabrandt/udemy-feature-engineering">
    <img src="logo.png" alt="Logo">
  </a>

  <h3 align="center">Udemy: Feature Engineering</h3>

  <p align="center">
    Code repository for Udemy course
    <br />
    <a href="https://github.com/sophiabrandt/udemy-feature-engineering"><strong>Explore the docs »</strong></a>
    <br />
    <br />
    <a href="https://github.com/sophiabrandt/udemy-feature-engineering">View Demo</a>
    ·
    <a href="https://github.com/sophiabrandt/udemy-feature-engineering/issues">Report a Bug</a>
    ·
    <a href="https://github.com/sophiabrandt/udemy-feature-engineering/issues">Request Feature</a>
  </p>
</p>

<!-- TABLE OF CONTENTS -->

## Table of Contents

- [About the Project](#about-the-project)
  - [Built With](#built-with)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
- [Usage](#usage)
- [Roadmap](#roadmap)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)
- [Acknowledgements](#acknowledgements)

<!-- ABOUT THE PROJECT -->

## About The Project

The project serves as a backup and online wiki for the lectures in the Udemy course **[Feature Engineering for Machine Learning][udemy]** by Soledad Galli.

### Built With

- [Docker](https://www.docker.com/) and docker-compose
- Python
- [Jupyter Notebooks](https://jupyter.org/)

<!-- GETTING STARTED -->

## Getting Started

To get a local copy up and running follow these steps:

### Prerequisites

You'll need Docker and docker-compose:

- Docker

```sh
docker --version
> Docker version 19.03.5-ce
```

- docker-compose

```sh
docker-compose -v
> docker-compose version 1.25.3
```

### Installation

1. Clone the repo

```sh
git clone https://github.com/sophiabrandt/udemy-feature-engineering.git
```

2. Create `.env_dev` file with the following format:

```
# credentials and database information
db_username=test_username
db_password=test_password
db_host=test_host
db_port=test_port
db_name=test

# disables lag in stdout/stderr output
PYTHONUNBUFFERED=1
PYTHONDONTWRITEBYTECODE=1

# random seed
random_seed=42
```

3. Build and run container

```sh
docker-compose up --build -d
```

<!-- USAGE EXAMPLES -->

## Usage

_Note:_ The Jupyter Notebook uses Vim key mappings for developent. See [Dockerfile-dev](docker/Dockerfile-dev). Delete relevevant lines in the Dockerfile if needed.

1. Go to `http://localhost:8008` for JupyterLab. Enter access token: `local_dev`.

2. Develop and save any notebooks into `/notebooks`. Save final artifacts/models needed for production in `/code`.

3. Save final version of code and any models the code relies upon into `/code`.

<!-- ROADMAP -->

## Roadmap

See the [open issues](https://github.com/sophiabrandt/udemy-feature-engineering/issues) for a list of proposed features (and known issues).

<!-- CONTRIBUTING -->

## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

<!-- LICENSE -->

## License

Distributed under the BSD-3-Clause License. See [`LICENSE`](LICENSE.txt) for more information.  
Original code by Soledad Galli. Original Docker setup by Binal Patel.

<!-- CONTACT -->

## Contact

Sophia Brandt - [@hisophiabrandt](https://twitter.com/hisophiabrandt)

Project Link: [https://github.com/sophiabrandt/udemy-feature-engineering](https://github.com/sophiabrandt/udemy-feature-engineering)

<!-- ACKNOWLEDGEMENTS -->

## Acknowledgements

- [Feature Engineering for Machine Learning][udemy] by Soledad Galli
- [Data Science Docker Template](https://github.com/caesarnine/data-science-docker-template) by Binal Patel

<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->

[contributors-shield]: https://img.shields.io/github/contributors/sophiabrandt/udemy-feature-engineering.svg?style=flat-square
[contributors-url]: https://github.com/sophiabrandt/udemy-feature-engineering/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/sophiabrandt/udemy-feature-engineering.svg?style=flat-square
[forks-url]: https://github.com/sophiabrandt/udemy-feature-engineering/network/members
[stars-shield]: https://img.shields.io/github/stars/sophiabrandt/udemy-feature-engineering.svg?style=flat-square
[stars-url]: https://github.com/sophiabrandt/udemy-feature-engineering/stargazers
[issues-shield]: https://img.shields.io/github/issues/sophiabrandt/udemy-feature-engineering.svg?style=flat-square
[issues-url]: https://github.com/sophiabrandt/udemy-feature-engineering/issues
[license-shield]: https://img.shields.io/badge/License-BSD%203--Clause-blue.svg
[license-url]: https://github.com/sophiabrandt/udemy-feature-engineering/blob/master/LICENSE.txt
[product-screenshot]: images/screenshot.png
[udemy]: https://www.udemy.com/course/feature-engineering-for-machine-learning/
