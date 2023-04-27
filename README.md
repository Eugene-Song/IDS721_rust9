# Rust week9 mini project
This is a simple Rust-based command-line tool that searches a specified path for duplicate files. The tool compares the performance of serial and parallel versions of the program.

## Prerequiste
This project is basde on Noah Gift's mlops template. And for testing data can be found in his repo. This repo does not include any test data. For testing, you have to use your own data for testing.

## Features

Search for duplicate files in a given directory. Compare the performance of serial and parallel implementations. Display duplicate files grouped by their checksums
## Dependencies
Rust 1.54.0 or later
clap library for parsing command-line arguments

## Installation
Clone this repository:

```git clone https://github.com/user/repo.git```
``` cd repo ```

## Usage
``` parallel parallel --path /src/data/```

The command-line tool provides two subcommands:

parallel: Search for duplicate files using the parallel implementation
serial: Search for duplicate files using the serial implementation
Both subcommands accept an optional -p or --path flag, followed by the path of the directory you want to search for duplicate files. If the flag is not provided, the default path is src/data/.

### Search for duplicate files using the parallel version
./target/release/duplicate_file_finder parallel -p /path/to/directory

### Search for duplicate files using the serial version
./target/release/duplicate_file_finder serial -p /path/to/directory
The output will display a list of duplicate files, grouped by their checksums.

## License
This project is licensed under the MIT License - see the LICENSE file for details.
## References
* [rust-cli-template](https://github.com/kbknapp/rust-cli-template)
