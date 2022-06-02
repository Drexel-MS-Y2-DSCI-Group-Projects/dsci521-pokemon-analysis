## Pokemon Color Analysis
dsci521-pokemon-analysis contains code that analyzes the aggregated data for Pokemon colors and types.

## Team Members

- Joseph Lunine: jel99@drexel.edu
- Owen Marett: om337@drexel.edu
- Evan Radcliffe: emr76@drexel.edu
- Jiangyan Shi: js4986@drexel.edu

## Getting Started
Prerequisite: Python 3

### Running the project
1. `python -m pip install -r requirements.txt`
2. Check out each individual analysis folder for a README on how to run it

### Dependency highlights

**pandas**

For representing html table data to convert to json. Used in bulbapedia scraping.

**opencv-python**

For modifying image data during color parsing. We reshape scraped images and convert to RGB color space.

**scikit-learn**

We use k-Means clustering algorithm to find the top colors of a pokemon image, provided by the scikit learn library.

**numpy**

For representing image data as higher performance arrays during image decoding and color picking.

**beautifulsoup4**

For scraping all relevant data from each of our data sources.

**lxml**

This subdependency is required for the pandas read_html function to convert html tables into DataFrames.

**PIL**

This dependency is used to do the conversion from hex code to RGB color.

**webcolors**

A library for CSS colors and converting from hex to RGB

**scipy**

Also part of the color analysis, used to find the closest CSS color name a RGB color corresponds to

**tqdm**

Used to time the processing of the image analysis piece

### Standard library dependencies

**json**

JSON is our data format of choice. In intermediate steps it contains each module's data. This is how our final data is also stored.

**requests**

Capturing html from the web. Stringified HTML must be passed to BeautifulSoup.

**time**

Timing the runner provides additional insight during runs for the data scraping process.

**re**

Regex helps parse tables during bulbapedia scraping only containing pokemon data.

**getopt**

Command line parser tool for simplifying the query input processing.

**os**

For creating data folder to store data as csv file.

## Sources
- [PokeAPI](https://pokeapi.co/docs/v2)
- [Bulbapedia](https://bulbapedia.bulbagarden.net/wiki/List_of_Pok%C3%A9mon_by_National_Pok%C3%A9dex_number)
- [PokemonDB](https://pokemondb.net/pokedex/all)
