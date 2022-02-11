# versioner
A small tool to automatically tag a repository based on the last commit message

## Installation

### From source

```
go install github.com/siklol/versioner/cmd/versioner
```

## Usage

After installation, you can run versioner inside of a repository. It expects one of the following tokens inside the commit message:

```
[patch] => v0.0.1
[minor] => v0.1.0
[major] => v1.0.0
```

### Dryrun

```
versioner
```

To show more extensive logs you can use the environment variable LOG_LEVEL.

### Force - write tag

```
versioner -f
```