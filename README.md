Screwdriver in a Box
====================

[![GitHub Workflow Status][GitHub Workflow Status]](https://github.com/QubitPi/screwdriver-cd-in-a-box/actions/workflows/ci-cd.yml)
![Last Commit](https://img.shields.io/github/last-commit/QubitPi/screwdriver-cd-in-a-box/master?logo=github&style=for-the-badge)
[![License Badge]](./LICENSE)

This handy feature will bring up an entire Screwdriver instance (UI, API, and log store) locally for us to play with. 
All data written to a database will be stored in `data` directory.

Quickstart
----------

Requires:

- Python 2.7.11+
- [Docker]
- [Docker Compose 1.8.1+][docker-compose]

1. [Login to Docker](https://docs.docker.com/engine/reference/commandline/login) with your Docker username (not
   email) or install [Docker Desktop]
2. Run the below command in the terminal to bring up a Screwdriver cluster locally.

   ```bash
   git clone https://github.com/QubitPi/screwdriver-cd-in-a-box.git
   cd screwdriver-cd-in-a-box
   python3 setup.py
   ```

3. We will be prompted to enter our desired SCM provider as well as our Client ID and Client Secret. Afterwards, type
   `y` to launch Screwdriver!

Documentation
-------------

- [screwdriver-cd-in-a-box](https://qubitpi.github.io/screwdriver-cd-guide/cluster-management/running-locally)
- [Cluster setup](https://qubitpi.github.io/screwdriver-cd-guide/cluster-management/kubernetes) (not in-a-box anymore)

[Docker]: https://www.docker.com/products/docker
[docker-compose]: https://www.docker.com/products/docker-compose
[Docker Desktop]: https://www.docker.com/products/docker-desktop/

[GitHub Workflow Status]: https://img.shields.io/github/actions/workflow/status/QubitPi/screwdriver-cd-in-a-box/ci-cd.yml?branch=master&logo=github&style=for-the-badge

[License Badge]: https://img.shields.io/badge/license-BSD%203--Clause-blue.svg?style=for-the-badge
