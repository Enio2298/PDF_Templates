# PDF_Templates
Generate PDF based in predefined guidelines

This Python program generates a multi-page PDF portfolio from topics specified in a CSV file. Each page in the PDF is styled with a header, footer, and lined sections to help organize notes or content. The program uses the `fpdf` library to create the PDF and `pandas` to read and process the topics.

## Features
- Creates a PDF with a title page for each topic and additional pages as specified.
- Adds horizontal lines for structured writing or note-taking.
- Customizable font styles, colors, and page layout.

## Requirements
- Python 3.x
- [fpdf](https://pyfpdf.github.io/fpdf2/)
- [pandas](https://pandas.pydata.org/)

## Installation
1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/portfolio-pdf-generator.git

Navigate to the project directory:

cd portfolio-pdf-generator

Install the required packages:

    pip install fpdf pandas

Usage

    Prepare the CSV File:
        The CSV file should be named topics.csv and placed in the same directory as the program.
        The CSV should contain at least two columns:
            Topic: Title of the section.
            Pages: Number of pages for that topic.

    Example topics.csv:

Topic,Pages
Introduction,3
Data Analysis,5
Machine Learning,4

Run the Program:

    In the terminal, run the program:

        python portfolio_generator.py

        This will generate an output.pdf file in the same directory.

Code Explanation

    Page Setup:
        The program initializes an FPDF object with portrait orientation, millimeter units, and A4 format.
        Automatic page breaks are disabled to allow full control over pagination.

    Main Loop:
        For each topic in the CSV, a title page is added with the topic name as a header.
        Additional pages are created based on the specified number of pages for each topic.
        Horizontal lines are added to each page for structured note-taking.

    Footer:
        Each page includes a footer with the topic name for easy reference.

Example Output

    output.pdf: A multi-page PDF file with headers and lined pages for each topic.

Contributing

Feel free to submit issues or contribute to this project by forking the repository and submitting a pull request.
