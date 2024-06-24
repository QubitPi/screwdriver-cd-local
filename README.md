Running Screwdriver Locally
===========================

[![GitHub Workflow Status badge][GitHub Workflow Status badge]][GitHub Workflow Status URL]
![Last Commit](https://img.shields.io/github/last-commit/QubitPi/screwdriver-cd-in-a-box/master?logo=github&style=for-the-badge)
[![License Badge]](./LICENSE)

This handy feature will bring up an entire Screwdriver instance (UI, API, and log store) locally for us to play with. 
All data written to a database will be stored in `data` directory.

Quickstart
----------

1. [Install Docker]
2. [Install Docker Compose][Docker Compose v2]
3. Run the command below in the terminal to bring up a Screwdriver cluster locally.

   ```bash
   docker pull node:18
   docker pull buildpack-deps:22.04-scm

   git clone https://github.com/QubitPi/screwdriver-cd-local.git
   cd screwdriver-cd-local
   python3 setup.py
   ```

4. You will be prompted to enter your desired SCM provider as well as the Client ID and Client Secret. Afterwards, type
   `y` to launch Screwdriver!

Documentation
-------------

- [Running Screwdriver in Docker Compose](https://screwdriver-docs.qubitpi.org/cluster-management/docker-compose)
- [Cluster setup](https://screwdriver-docs.qubitpi.org/cluster-management/kubernetes) (__not local anymore__)

[Install Docker]: https://github.com/QubitPi/docker-install
[Docker Compose v2]: https://stackoverflow.com/a/66516826/14312712

[GitHub Workflow Status badge]: https://img.shields.io/github/actions/workflow/status/QubitPi/screwdriver-cd-local/ci-cd.yml?branch=master&logo=github&style=for-the-badge
[GitHub Workflow Status URL]: https://github.com/QubitPi/screwdriver-cd-local/actions/workflows/ci-cd.yml

[License Badge]: https://img.shields.io/badge/license-BSD%203--Clause-blue.svg?style=for-the-badge
