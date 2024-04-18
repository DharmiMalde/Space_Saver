# Space Saver Project

## Overview

The Space Saver Project is a web scraping tool designed to extract addresses from web pages, using a series of pattern identification techniques to optimize space and enhance readability. This project aims to streamline the process of retrieving address information from various web sources for efficient data analysis or utilization in other applications.

## Features

- **Pattern Identification**: Employs pattern identification techniques to identify and extract addresses from web pages.
- **Content Optimization**: Removes extraneous content to focus solely on address information, enhancing readability and space efficiency.
- **Customizable**: Offers options for customization to adapt to different address formats and web page structures.
- **Efficient**: Provides a fast and efficient way to extract address data from multiple web pages without manual intervention.

## Pattern Identification Steps

1. **Step 1: Address Segmentation**: Iterates through each comma in the files, keeping at most seven words on each side of it until the next and previous comma, omitting the rest if there were more than seven.

2. **Step 2: Capitalization Check**: Goes through consecutive blocks of four words and omits the block if there are no capitalized words in it, as most words in addresses are capitalized.

3. **Step 3: Word Probability Filtering**: Creates a list of words with a very low probability of appearing in addresses and omits all those words from the file if present.
