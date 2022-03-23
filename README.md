# DecimalTools
A Mendix module to parse various formats of decimal strings into Mendix Decimal values.

Decimals can be written in a number of formats, but the built in ParseDecimal function only allows for the format associated with your locale to be parse. This module gives you the ability to parse decimals from other formats outside your locale.

## Usage

ParseDecimal

* Decimal - The decimal in string format. e.g. '1,234.56'
* Format - the format of the decimal, usually you will just want to set this to '#,##0.0#'. See [DecimalFormat](https://docs.oracle.com/javase/7/docs/api/java/text/DecimalFormat.html) for more options.
* DecimalSeparator - the character to use to represent the decimal separator. e.g. '.'
* GroupingSeparator - the character to use to represent the grouping separator. e.g ','

The action can throw an error if it bad values are pass to it, so remember to set error handling to catch and handle this appropriately.

## Contributing
The source code, examples, and unit tests can be found on [https://github.com/robertprice/DecimalTools](https://github.com/robertprice/DecimalTools).

## Author
Robert Price - [Deck Chair Digital Ltd](https://deckchair.digital/).
