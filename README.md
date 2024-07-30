### README.md for Coursework Assignment 1

# Coursework Assignment 1: Dual_EC_DRBG Exploit

## Overview

This project is part of the CO3326 Computer Security coursework for the academic year 2023-2024. It involves the implementation and analysis of the Dual Elliptic Curve Deterministic Random Bit Generator (Dual_EC_DRBG) algorithm, including the creation of a backdoor similar to that alleged in the NSA exploit.

## Table of Contents

- [Overview](#overview)
- [Files](#files)
- [Getting Started](#getting-started)
- [Assignment Details](#assignment-details)
- [Implementation](#implementation)
- [Usage](#usage)
- [References](#references)

## Files

- `Assignment/`
  - `Coursework assignment.pdf`
- `CO3326cw1.docx`
- `CO3326cw1.json`
- `CO3326cw1.pdf`
- `DualECExploit.py`

## Getting Started

1. **Clone the Repository**

   ```sh
   git clone https://github.com/isbethwel/Coursework-assignment-1-2023-2024.git
   cd Coursework-assignment-1-2023-2024
   ```

2. **Set Up the Environment**

   Ensure you have Python and the required libraries installed:

   ```sh
   pip install ecdsa
   ```

## Assignment Details

### Part A - Exercise

You are required to:

1. Generate a sequence of five pseudorandom numbers starting from an initial state.
2. Extrapolate the next three pseudorandom numbers from two intercepted pseudorandom numbers using a built-in backdoor.

### Part B - Report

The report (`CO3326cw1.pdf`) answers key questions related to elliptic curve cryptography, the discrete logarithm problem, and the Dual_EC_DRBG algorithm. It also provides detailed explanations and diagrams to support the answers.

## Implementation

The implementation involves two main components:

1. **Dual_EC_DRBG Algorithm**

   The `DualECExploit.py` script implements the Dual_EC_DRBG algorithm using elliptic curve cryptography. It includes functions for generating pseudorandom numbers and exploiting the backdoor.

2. **Backdoor Exploit**

   The backdoor exploit allows prediction of future pseudorandom numbers given two intercepted numbers and a known backdoor factor.

## Usage

1. **Run the Script**

   To generate pseudorandom numbers and predict future numbers using the backdoor:

   ```sh
   python DualECExploit.py
   ```

2. **View the Output**

   The script will output the generated pseudorandom numbers and the predicted numbers using the backdoor.

## References

1. Boneh, D. and Shoup, V., 2020. A graduate course in applied cryptography. Draft 0.5.
2. Hankerson, D. and Menezes, A., 2021. Elliptic curve cryptography. In Encyclopedia of Cryptography, Security and Privacy (pp. 1-2). Berlin, Heidelberg: Springer Berlin Heidelberg.
3. Koblitz, N., 1994. A course in number theory and cryptography (Vol. 114). Springer Science & Business Media.
4. PUB, F., 2000. Digital signature standard (DSS). FIPS PUB, pp.186-192.
5. Silverman, J.H., 2009. The arithmetic of elliptic curves (Vol. 106, pp. xx+-513). New York: Springer.
6. Washington, L.C., 2008. Elliptic curves: number theory and cryptography. CRC press.