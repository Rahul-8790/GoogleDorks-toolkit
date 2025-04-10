# GoogleDorks Toolkit

![GoogleDorks Toolkit](https://github.com/Rahul-8790/GoogleDorks-toolkit/blob/a61b7d6f6b30186a92d94e5d5c59463580b58318/GoogleDorks-toolkit-main/GoogleDorks-toolkit-main/Image.png)

GoogleDorks Toolkit is a Python script designed to help security researchers and penetration testers automate Google dorking for finding potential vulnerabilities and information about a target domain. The tool utilizes Google search queries, also known as Google hacks, to identify possible security issues and gather valuable information.

## Features

- **Customizable Dorks**: Users can provide their own list of dorks to be used in the Google search queries with huge list of default Google Dorks list.
- **Domain Search**: The tool allows users to specify a target domain for the Google dorking process.
- **Results Output**: Search results are saved to an output file, providing a convenient way to review and analyze the findings.
- **Detailed Results**: Not only the vulnerable webapps and the dork, but also the auther and reference link of the dork for more information.
- **Vulnerability Disclosure and Bug Bounty Checker**: Optional detection of vulnerabilities by searching for the identified domains in existing file `OpenForReport.txt` which own VDP or BBP programs to report legally.

## Usage

## Prerequisites

- Python 3.x
- Required Python packages: `googlesearch`, `enum`, `argparse`, `pyfiglet`

## Installation



```
chmod +x setup.sh
./setup.sh
```

### Kali Linux
```
apt update; apt upgrade
git clone https://github.com/Rahul-8790/GoogleDorks-toolkit.git
cd google-dorks-toolkit
```
### Termux
```
pkg update; pkg upgrade
git clone https://github.com/Rahul-8790/GoogleDorks-toolkit.git
cd GoogleDorks-toolkit
cd GoogleDorks-toolkit-main
ls
chmod +x setup.sh
./setup.sh
python GoogleDorks-toolkit.py

```


## Command-line Arguments

    - `-d`, `--domain`: Specify the target domain for Google dorking (required).
    - `-n`, `--number_of_pages`: Set the number of pages to search (required).
    - `-t`, `--time`: Specify the time between requests to avoid being blocked by Google (required).
    - `-o`, `--output`: (Optional) Specify the output file name for saving the results.
    - `--search`: (Optional) Search matched domains in OpenForReport.txt, note that the output should be yes or y only.
    - `-l`, `--list`: (Optional) Add your own dorks list.

## Example
```
python GoogleDorks-toolkit.py -d example.com -n 5 -t 5 -o results.txt --search yes
```

## Developers

-Rahul limbad

## Note

This tool is intended for educational and ethical use only. Use it responsibly and ensure compliance with applicable laws and regulations.
## Disclaimer

The developers are not responsible for any misuse or damage caused by this script. Use it at your own risk.

