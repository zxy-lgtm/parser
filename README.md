# Parser - A MySQL Compatible SQL Parser

The goal of this project is to build a Golang parser that is fully compatible with MySQL syntax, easy to extend, and high performance. Currently, features supported by parser are as follows:

- Highly compatible with MySQL: it supports almost all features of MySQL. For the complete details, see [parser.y](https://github.com/arana-db/parser/blob/dev/parser.y) and [hintparser.y](https://github.com/arana-db/parser/blob/dev/hintparser.y).
- Extensible: adding a new syntax requires only a few lines of Yacc and Golang code changes. As an example, see [PR-9](https://github.com/arana-db/parser/pull/9/files).
- Good performance: the parser is generated by goyacc in a bottom-up approach. It is efficient to build an AST tree with a state machine.

## Future

- Support more MySQL syntax
- Optimize the code structure, make it easier to extend
- Improve performance and benchmark
- Improve the quality of code and comments

## License
Parser is under the Apache 2.0 license. See the LICENSE file for details.

