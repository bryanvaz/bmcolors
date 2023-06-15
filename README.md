# README.md

## Benjamin Moore Color Collections Scraper (bmcolors)

This Python program scrapes the Benjamin Moore website to get all available color collections, download the associated ASE files, and parse the ASE files to extract color data. The parsed color data is then saved to a workspace directory in both YAML and JSON formats.

### Prerequisites

This program uses the `pipenv` tool for managing its dependencies. You will need to have `pipenv` installed on your system to run the program. If you don't have `pipenv` installed, you can install it using pip:

```bash
pip install pipenv
```

### Installation

To install the dependencies of the program, navigate to the program directory and run:

```bash
pipenv install
```

This command will create a virtual environment and install all the dependencies specified in the `Pipfile`.

### Running the Program

You can run the program using the following command:

```bash
pipenv run bmcolors
```

This command will run the main function of the program. 

By default, the program will scrape the Benjamin Moore website, download the ASE files, and parse the ASE files to extract color data.

### Command Line Arguments

The program supports the following command line arguments:

- `--scrape`: Scrape the Benjamin Moore website to get all available color collections and download the ASE files.
- `--parse`: Parse all ASE files in the workspace and save the parsed color data (no download).
- `--all`: Scrape the Benjamin Moore website, download the ASE files, parse the ASE files, and save the parsed color data.

For example, to only parse the ASE files in the workspace, you would run:

```bash
pipenv run bmcolors --parse
```

### Output

The parsed color data is saved in the `workspace` directory in the root of the project directory. The color data is saved in two formats:

- YAML file (`benjaminmoore-colors.yaml`)
- JSON file (`benjaminmoore-colors.json`)

Each file contains a dictionary where the keys are the names of the color collections and the values are lists of color data.

### Contributing

Contributions are welcome. Please fork the repository and submit a pull request with your changes.

### License

This project is licensed under the MIT License. See the `LICENSE` file for more information.