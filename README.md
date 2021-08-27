grepgithub
----------
Command line util for grep.app - Search across a half million git repos

![Screenshot](https://raw.githubusercontent.com/popovicn/images/master/grepgithub/screenshot.png)

Grepgithub uses [grep.app](https://grep.app/) API to search GitHub repositories, 
providing colorful CLI or JSON output format suitable for integration and automation.  

Try making your search as specific as possible because API returns only first 1000 matches.  
Request are delayed and search can last up to 2 minutes. 


### Usage
```
usage: grepgithub.py [-h] -q QUERY [-c] [-r] [-w] [-frepo REPO_FILTER] [-fpath PATH_FILTER]
                     [-flang LANG_FILTER] [-json] [-o OUTPUT_FILE]

optional arguments:
  -h, --help          show this help message and exit
  -q QUERY            Query string, required
  -c                  Case sensitive search
  -r                  Use regex query. Cannot be used with -w
  -w                  Search whole words. Cannot be used with -r
  -frepo REPO_FILTER  Filter repository
  -fpath PATH_FILTER  Filter path
  -flang LANG_FILTER  Filter language (eg. Python,C,Java). Use comma for multiple values
  -json               JSON output
  -o OUTPUT_FILE      Output file path
```