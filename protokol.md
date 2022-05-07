## Scenario
The CISO of a large company wants to implement a vulnerability management system, but there are too many subnets and firewalls to handle assessment manually, so there's a need for program that assigns subnets to an accessible vulnerability scanner and splits responsibility between daughter companies.

There are 3 sources of input data:
* Table of network subnets
* Table of IP addresses of vulnerability scanners
* Table of rules that modify subnet assignment and apply filters

At the end, CISO can validate that all subnets are assigned to the scanner.

## Requirements

1. Input data can be imported as a bundle and modified in GUI
2. Processing is resource hungry, so users have to create a list of rules, that are applied after a button click.
3. CISO can see if there's any problem with subnet assignment (unassigned subnets, vulnerability scanners)
4. Data can be exported for use of vulnerability management tool.

## Technology utilized

* Python 3
* SQLite
* GTK

## Time schedule

* 6h app architecture
* 2h db setup
* 4h data model
* 6h controller
* 4h debug code
* 4h loading data from file
* 6h gui baseline
* 2h gui input
* 2h gui export
* 4h debug code