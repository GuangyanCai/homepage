# Guide

## Dependencies

Install scoop:
```bash
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
iwr -useb get.scoop.sh | iex
```
Install dependencies:
```bash
scoop install git go hugo-extended nodejs pipx
```

For importing publications (make sure python>=3.11.5):
```bash
pip install academic
```

## View
```bash
hugo server -D
```

## Import publications
```bash
academic import publications.bib content/publication/ --compact
``` 
