# yammer report deviceusageusercounts

Gets the number of daily users by device type

## Usage

```sh
m365 yammer report deviceusageusercounts [options]
```

## Options

Option|Description
------|-----------
`--help`|output usage information
`-p, --period <period>`|The length of time over which the report is aggregated. Supported values `D7,D30,D90,D180`
`--query [query]`|JMESPath query string. See [http://jmespath.org/](http://jmespath.org/) for more information and examples
`-o, --output [output]`|Output type. `text,json`. Default `text`
`--verbose`|Runs command with verbose logging
`--debug`|Runs command with debug logging

## Examples

Gets the number of daily users by device type for the last week

```sh
m365 yammer report deviceusageusercounts --period D7
```

Gets the number of daily users by device type for the last week and exports the report data in the specified path in text format

```sh
m365 yammer report deviceusageusercounts --period D7 --output text > "deviceusageusercounts.txt"
```

Gets the number of daily users by device type for the last week and exports the report data in the specified path in json format

```sh
m365 yammer report deviceusageusercounts --period D7 --output json > "deviceusageusercounts.json"
```
