# Demo of od2net


The in this repo is intended to demonstrate how to use
[`od2net`](https://github.com/Urban-Analytics-Technology-Platform/od2net)
to generate route networks and to compare the workflow, and results,
with the R-based approach currently used in the NPT project.

# od2net minimum example

The following is based on [`od2net`’s
docs](https://github.com/Urban-Analytics-Technology-Platform/od2net/blob/main/docs/tutorial_examples.md#running-the-edinburgh-example)
and the code in the examples/edinburgh folder.

Setup the files in the input folder as follows:

``` r
source("R/setup.R")
main()
```

Run the tool with Docker as follows:

``` bash
docker run -v $(pwd):/app ghcr.io/urban-analytics-technology-platform/od2net:main /app/config.json
```

After that you should see the following in the output folder:

``` r
fs::dir_tree("output")
```

    output
    ├── counts.csv
    ├── output.geojson
    └── rnet.pmtiles

## Setup

Run the code on a computer with Ubuntu 22.04 after running the setup
outlined in the link above.

``` bash
gh repo clone Urban-Analytics-Technology-Platform/od2net
# Copy the example to this folder:
cp -r od2net/examples/edinburgh/* .
cp -r od2net/
```
