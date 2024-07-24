<img style='border: 1px solid black' align="right" width="300" src="https://raw.githubusercontent.com/euctrl-pru/HexAeroPy/main/assets/hexaeropy_logo.png" alt="HexAeroPy logo" />

# HexAeroSpark

HexAero is a EUROCONTROL Python, PySpark and R package designed for aviation professionals and data analysts. It allows for the determination of used airports, runways, taxiways, and stands based on available (ADS-B) flight trajectory coordinates. This tool aims to enhance aviation data analysis, facilitating the extraction of geospatial milestones for operational performance analysis.

The package is built on top of the H3 system developed by Uber Technologies, Inc. and open geospatial data retrieved from OpenStreetMap (OSM) and OurAirports.com. H3 is a hexagonal hierarchical geospatial indexing system that enables coordinates to be associated with hexagons (identified by an H3 tag). The hexagons used in this indexing system cover the Earth's surface in various resolutions (i.e., hexagon sizes). By labelling and thus associating certain hexagons (i.e., H3 tags) to various spatial features (e.g., airports, stands, taxiways, runways, or other regions extracted from OSM and OA), one can detect the flight trajectory entry and exit of these regions. In practice, this is done by transferring the (ADS-B) trajectory coordinates (latitude, longitude) to the associated hexagons covering the trajectory (i.e., by determining the H3 tags of the flight coordinates) and associating these to the predefined hexagons covering the geospatial feature of interest.

## To do list for developers
1. Update code to generate airport layouts to use `osmnx` and `geopandas`. See code `python\create_h3_data_airport_layout.py`. 
2. Write code to upload generated airport layout datasets to Hive / Impala / .... whichever storage.
3. Implement trajectory labelling algorithm.
4. Write post labelling/processing logic.   

## Installation [TBD]

To install HexAeroSpark, ensure you have Python 3.9+ installed. Then run the following command:

``` bash
pip install HexAeroSpark
```

## Quick Start [TBD]

Get started with HexAeroPy by running the following Python code: [TBD]

## Usage [TBD]

## Development Roadmap [TBD]

## Contributing

We welcome contributions to HexAeroPy! Feel free to submit pull requests, report issues, or request features.

## License

HexAeroPy is licensed under the MIT License - see the [LICENSE](https://github.com/euctrl-pru/HexAeroPy/blob/main/LICENSE) file for details.

## Credits and Acknowledgments

Special thanks to ...
- [EUROCONTROL](https://www.eurocontrol.int/)
- [Performance Review Commission (PRC)](https://ansperformance.eu/about/prc/)
- [European Connected Regional Airports (ECRA) Initiative](https://www.eurocontrol.int/service/european-connected-regional-airports)

## Contact Information

For support or queries, please contact us at [pru-support@eurocontrol.int](mailto:pru-support@eurocontrol.int).
