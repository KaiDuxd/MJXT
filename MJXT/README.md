# JXT & JXT+ & JXT++

This repo implements the join query schemes, for example, JXT [1], JXT+ and JXT++, and shows the constructions and comparison of them. 

## Table of Contents

- [Background](#background)
- [Features](#features)
- [Installation](#installation)
  - [Prerequisites](#prerequisites)
  - [Clone Repository](#clone-repository)
  - [Build](#build)
- [Usage](#usage)
  - [Overview](#overview)
  - [Getting Started](#getting-started)
  - [Build Project](#build-project)
  - [Run Experiments](#run-experiments)
  - [Validate Results](#validate-results)
  - [Reuse Beyond the Paper](#reuse-beyond-the-paper)
- [Contribution](#contribution)
- [License](#license)
- [Contact Information](#contact-information)

## Background

The corresponding works i.e., JXT, JXT+, JXT++, solve the join query over encrypted database. The project aims to implement JXT, JXT+ and JXT++ by JAVA, and show the comparison of their storage overhead and query efficiency. 

## Features

- Applied Cryptography
- Encrypted Database
- Join Queries
- JAVA

## Installation

### Prerequisites

- A computer (Recommended configuration 16 GB RAM)
- JDK version 1.8.0
- Maven

### Clone Repository

```bash
git clone https://github.com/yourusername/your-repo-name.git
cd your-repo-name
```

# Build

Build the project using Maven:

```
mvn clean install
```

## Usage

### Overview

- [Getting Started](https://idealab.alibaba-inc.com/ideaTalk#getting-started) (10 human-minutes + 5 compute-minutes)
- [Build Project](https://idealab.alibaba-inc.com/ideaTalk#build-project) (2 human-minutes + 1 compute-hour)
- [Run Experiments](https://idealab.alibaba-inc.com/ideaTalk#run-experiments) (5 human-minutes + 3 compute-hours)
- [Validate Results](https://idealab.alibaba-inc.com/ideaTalk#validate-results) (30 human-minutes + 5 compute-minutes)
- [Reuse Beyond the Paper](https://idealab.alibaba-inc.com/ideaTalk#reuse-beyond-the-paper) (20 human-minutes)

### Getting Started (10 human-minutes + 5 compute-minutes)

1. Follow the instructions at XYZ to run our VM/container (10 minutes read).

2. Run

    

   ```
   ./install.sh
   ```

    

   and go grab a coffee (5 minutes to install).

   - You will see no output while the script runs.
   - The script accesses the internet to download external dependencies such as Qux and Baz.
   - Once complete, it will have created a directory called `stuff`.
   - If this command fails, you can delete the `stuff` directory and try again.

### Build Project (2 human-minutes + 1 compute-hour)

1. Run

    

   ```
   ./build.sh stuff
   ```

    

   and take a break—this will take ~1 hour to complete.

   - You should see a progress bar while the command runs.
   - Once complete, it will have created a `BUILD` directory.
   - If the `BUILD` directory already exists, it will be overwritten.

### Run Experiments (~3 compute-hours)

1. Run `./exp.sh 6 30m 1` to run our tool on only *6 benchmarks* for *30 minutes each* with only *1 repetition*.
   - This command takes only **3 hours** to run in total, and produces results that approximate the results shown in the paper.
   - Since there is only 1 repetition, there will be no error bars in the final plots.
   - Results will be saved in a directory called `results`.
2. Run `./exp.sh 20 24h 10` to replicate the full experiments in the paper.
   - This command takes **200 days** to run 10 reps of all 20 benchmarks for 24 hours each.
   - Feel free to tweak the args to produce results with intermediate quality, depending on the time that you have.
   - Results will be saved in a directory called `results`.

### Validate Results (30 human-minutes + 5 compute-minutes)

1. The output of the experiments will validate the following claims:
   - Table 1: `results/tab1.csv` reproduces Table 1 on Page 5.
   - Figure 2: `results/plot2.pdf` reproduces the plot in Figure 2 on Page 8.
   - Page 7, para 3: "We outperform the baseline by 2x". See `results/comparison.csv`, where the second column (our performance) should have a value that is twice as much as the third column (baseline).
2. Our artifact does not validate the following claims:
   - On Page 8, we say X, but this cannot be validated without access to specialized hardware/people, so we leave it out of scope of artifact evaluation.

### Reuse Beyond the Paper (20 human-minutes)

1. This section describes how to run a single instance of your research tool or system for a specific use case.

## Contribution

Contributions are welcome! Please see our [CONTRIBUTING.md](https://idealab.alibaba-inc.com/CONTRIBUTING.md) for more details.

1. Fork the repository.
2. Create a new branch (`git checkout -b feature/AmazingFeature`).
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`).
4. Push to the branch (`git push origin feature/AmazingFeature`).
5. Open a Pull Request.

## License

Distributed under the MIT License. See `LICENSE` for more information.

## Contact Information

You can reach us at:

- Author: [Your Name](https://github.com/yourusername)
- Email: [your.email@example.com](mailto:your.email@example.com)

This README document adheres to your provided tips. It organizes the steps clearly and includes human and compute time estimates, explanations of side-effects, and descriptions of how to handle dependencies and potential issues. Additionally, it provides an outline for the reviewers to verify the claims made in your paper, ensuring a smooth evaluation process.

# Reference

[1] Charanjit Jutla and Sikhar Patranabis. 2022. Efficient searchable symmetric encryption for join queries. In International Conference on the Theory and Application of Cryptology and Information Security. Springer, 304–333.