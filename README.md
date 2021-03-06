# ordered-ast-traverse.js
Simple but flexible lexically ordered AST traversal with pre and post visitors.

Same as [ast-traverse](https://github.com/olov/ast-traverse) but instead of
visiting everything that looks like an AST node, nodes are visited according to
[ordered-esprima-props](https://github.com/olov/ordered-esprima-props/blob/master/ordered-esprima-props.js).

The result is that the AST traversal happens in lexical order, i.e. an
AST-traversal in this order will visit nodes in increasing source code
position. Tested with Esprima but should work for any Mozilla Parser API
compatible AST, see
https://developer.mozilla.org/en-US/docs/Mozilla/Projects/SpiderMonkey/Parser_API

## Usage and examples
See [ast-traverse README](https://github.com/olov/ast-traverse/blob/master/README.md)

## License
`MIT`, see [LICENSE](LICENSE) file.
