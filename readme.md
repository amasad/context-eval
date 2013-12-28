# context-eval

Simple execution context for node and the browser. In node it just creates a new
context and `runInContext` in that context and in the browser it creates an
iframe and hangs on to it until destroy is called.

install:

    npm install context-eval

Use with browserify or node.

to run the tests:

    npm test

test in browsers:

    npm install karma -g
    karma start


## new Context(sandbox)

`sandbox` is an object that would be shallowly copied into the execution context.

## Context#evaluate(code)

Evaluates code and returns result.

## Context#destory()

Does nothing in node but removes iframe in browser.


### License

MIT