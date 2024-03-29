# Car fuel consumptions and emissions 2000-2013

[![Goodtables](https://goodtables.io/badge/github/amercader/car-fuel-and-emissions.svg)](https://goodtables.io/github/amercader/car-fuel-and-emissions)


Cleaned-up and consolidated car fuel consumption and emissions data for years
2000 to 2013. Data is published by the [Vehicle Certification Agency](http://www.dft.gov.uk/vca/)
(VCA), an Executive Agency of the United Kingdom Department for Transport.

Data is available to download at [http://carfueldata.direct.gov.uk/downloads/default.aspx]().

It is assumed that the data is released under the [UK Open Government License](http://www.nationalarchives.gov.uk/doc/open-government-licence/version/2/).

For more details about the data, please check the information booklet
[http://carfueldata.direct.gov.uk/additional/aug2013/VCA-Booklet-text-Aug-2013.pdf]().

## Data Cleaning

The original data is published in separate CSV file starting from 2000, but
the format is not consistent across years. Data has been consolidated for
machine using [OpenRefine](http://openrefine.org). The script with the tasks
performed on the 2013 CSV files is included in the `scripts` folder. Some
example operations performed include:

* Consolidate different field names across different years
* Consolidate measure units for emissions data across different years
* Set proper field types to allow indexing and analysis (eg numeric fields)
* Normalize manufacturer and model descriptions
* Trim excess whitespace
* Fix encoding for special characters
* etc

Note that the resulting dataset does not include all fields in the original
data, only those deemed more relevant.

