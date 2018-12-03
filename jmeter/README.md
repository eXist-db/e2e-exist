# HSG JMeter Tests Readme

## Prerequisites

* Java
* Jmeter (tested with Version 3.2.x)

## Known Issues

we can store only one result / day because the plugin generates the .jtl files with a hard coded naming pattern starting with the date (but not datetime). We can investigate further on this if required.


## Usage
run the following commands to clean the workspace, run the test and to generate the result graph:

* ```mvn verify```
* ```mvn clean```
* ```mvn jmeter-graph:create-graph```

Afterwards the results of the jmeter testrun can be found in target/jmeter/results.

## Configuration

 Tell JMeter to store its results in an XML format in `user.properties` file or as command option

```config
jmeter.save.saveservice.output_format=xml
```

or

```shell
jmeter -Jjmeter.save.saveservice.output_format=xml -n -t $TEST_PLAN
```