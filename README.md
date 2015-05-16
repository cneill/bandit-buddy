# Bandit Buddy

Ever wanted a prettier report from [Bandit](https://wiki.openstack.org/wiki/Security/Projects/Bandit)? BAM! You got it!

If you don't like the default template/style, just create new files in `/resources/templates/` and `/resources/styles/`. Look at the defaults to see what variables you can play with.

## Installation

    pip install -r requirements.txt

## Usage

```bash
Usage:
    buddy.py INFILE [CONFIGFILE] [OUTFILE]
    buddy.py --help

Options:
    INFILE        Specify the file to read bandit results from (in JSON format)
    CONFIGFILE    Specify the file to load project settings from (in JSON format) [default: ./config.json]
    OUTFILE       Specify the file for results to be written to [default: ./results.html]
    --help        Print help message
```

## Example config.json file

```json
{
    "project_name": "Derp Project",
    "template": "default",
    "style": "default"
}
```
