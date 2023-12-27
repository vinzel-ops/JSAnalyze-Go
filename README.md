# JSAnalyze-Go

JSAnalyze with Go is a sophisticated and robust tool designed for in-depth analysis of JavaScript files. It efficiently identifies endpoints, URLs, and embedded secrets within these files. Leveraging multi-threading technology, JSAnalyze with Go conducts concurrent analysis of numerous JavaScript files, offering an invaluable resource for security researchers, bug bounty hunters, and software developers.

## Features

- Rapid download of JavaScript files from a predefined list of URLs.
- Concurrent analysis of multiple JavaScript files, facilitated by multi-threading.
- Comprehensive extraction of endpoints and URLs embedded within JavaScript files.
- Identification of hardcoded secrets, supported by a modifiable list of regular expression (regex) patterns.
- Generation of structured and detailed reports for each JavaScript file analyzed.

## Installation

1. **Repository Cloning**:
   ```
   git clone https://github.com/yourusername/JSAnalyze-with-Go.git
   ```
2. **Navigating to the Tool's Directory**:
   ```
   cd JSAnalyze-with-Go
   ```
3. **Dependency Installation**:
   ```
   go get -u
   ```

## Usage

```
Usage: ./JSAnalyze-with-Go [OPTIONS]

Options:
  -u, --urls string        Specify the file path containing JavaScript URLs
  -s, --secrets string     (Optional) Specify the file path for regex wordlist of hardcoded secrets
  -o, --output string      (Optional) Specify the output directory path (default: "./output")
  -t, --threads int        (Optional) Set the number of processing threads (default: 10)
  -h, --help               Display help information and exit
```

## Example

```
./JSAnalyze-with-Go -u urls.txt -s secrets.txt -t 20
```

This command initiates the analysis of JavaScript files listed in `urls.txt`, seeks hardcoded secrets using regex patterns in `secrets.txt`, and utilizes 20 threads for efficient processing.

---------------
### EDUCATION PURPOSE ONLY
©Vinzel-2023
