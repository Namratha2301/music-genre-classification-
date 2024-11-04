# Music Genre Classification using Federated Learning

Paper Link: https://link.springer.com/chapter/10.1007/978-981-19-7447-2_23

## Overview

This project aims to classify music genres from audio recordings using machine learning techniques, specifically employing federated learning to enhance data privacy. The classification is based on audio features extracted from 3-second audio segments of various genres.

## Table of Contents

- [Introduction](#introduction)
- [Setup](#setup)
- [Data Preparation](#data-preparation)
- [Model Training](#model-training)
- [Results](#results)
- [Future Work](#future-work)
- [License](#license)

## Introduction

Music genre classification is a challenging task that can be significantly improved using machine learning techniques. In this project, we leverage federated learning to enable model training across multiple clients without sharing sensitive audio data. The model aims to recognize and classify music into various genres, including blues, classical, country, disco, pop, hip-hop, metal, reggae, and rock.

## Setup

### Prerequisites

To run this project, ensure you have the following installed:

- Python 3.6 or higher
- Libraries:
  - `numpy`
  - `librosa`
  - `matplotlib`
  - `tensorflow`
  - `pandas`

You can install the required libraries using pip:

```bash
pip install numpy librosa matplotlib tensorflow pandas
