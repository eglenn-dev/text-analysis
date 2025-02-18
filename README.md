<div align="center"><h1>Scripture Analyser Documentation</h1></div>

<div align="center"><code><a href="https://youtu.be/t__eVNM220Y" target="_blank">Video Demonstration</a></code></div>

### Quick Links

-   [Origional Project Plan](./docs/plan.md)
-   [Questions to Answer](#questions)
-   [Files Needed](#files)
-   [Menu Overview](#menu)

## Updates

#### June 10, 2024

-   Updated Documentation
-   Added `compare_verses()` function to `scripture_analysis.py`
    -   Added functions to support this new function in `scripture_processing.py`

## Preface

This project is a CLI application that is designed to analyze the text of the Bible and other Religous texts. These texts were chosen becuase of their size, complexity, and structure, as well as the fact that they are in the public domain. The goal of this project is to use natural language processing (NLP) to analyze the text of these books and answer some questions about them.

## Questions <a name="questions"></a>

For this project there were two guiding questions that I set out to answer.

-   Which book references Jesus the most?
-   Which two books are most simelar to eachother?

In an effort to answer these questions I user natural language processing (NLP) to compare the books and verses to eachother, as well as perform named entity recognition (NER) to identify the names of people and places mentioned in the text.

## Files <a name="files"></a>

-   [`scripture_analysis.py`](./scripture_analysis.py)
    -   This file contains the CLI user interface, as well as the main function that are performing the analysis.
-   [`scripture_processing.py`](./scripture_processing.py)
    -   This file contains the functions that are used to process the text of the books and verses. Many of these functions are used to clean the text and prepare it for analysis, and are shared by primary funcitons in `scripture_analysis.py`.
-   [`data`](./data)

    -   [`/output`](./data/output)
        -   Processed data that was stored in a dictionary is saved as a `.json` file here.
    -   [`/processed`](./data/processed)

        -   Output files are saves as `.pkl` files in this directory.

    -   [`/scriptures`](./data/scriptures)
        -   The raw data for the scriptures is sotred in regulary and flat JSON files here.

## Menu Overview <a name="menu"></a>

This section will overview the menu with images. This is a terminal application, but much of the data is outputted into json files for later use. The menu is as follows:

### Main Menu

![Main Menu](./docs/img/menu.png)

### Most Popular Names Manu

![First menu](./docs/img/menu1.png)

### Most Popular Places Results

![First result](./docs/img/result1.png)

### Named Entity Recognition for Jesus Christ

![Second Result](./docs/img/result2.png)

### Most Similar Books Results (Ordered)

![Third Result](./docs/img/result3.png)
