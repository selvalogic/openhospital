# Open Hospital

This repository is used to assemble the portable (or all-in-one) packages of the [Open Hospital][openhospital] project, which you can download [here][releases].

## How to contribute

If you'd like to contribute to the Open Hospital project, please read [CONTRIBUTING.md][contributing].

## How to create Open Hospital packages

To create the Open Hospital packages,
make sure to have installed the following dependencies on a Linux machine:
_JDK 8+, Maven, asciidoctor-pdf, docker, docker-compose, zip, GNU make_.

Then follow these simple steps:

 1. Clone this repository:

        git clone https://github.com/informatici/openhospital

 2. Run the script that compiles the components of Open Hospital, and assembles the portable distributions:

        cd openhospital
        make
    
    You can also parallelize some make tasks by using the `-j` flag (e.g. `make -j4`)
    or use intermediate targets to build single parts of the distribution 
    (e.g. `make database.sql` to create the database dump).


 [openhospital]: https://www.open-hospital.org/
 [releases]: https://github.com/informatici/openhospital/releases
 [contributing]: https://github.com/informatici/openhospital/blob/master/CONTRIBUTING.md
