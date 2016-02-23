# example

A repo to store examples

# Graphviz

Graph Visualization Software [graphviz](http://www.graphviz.org/) is pretty
neat.

## Basic graph

Something like [hello.dot](hello.dot) is a basic graph:

```dot

graph G {
    va -- vb;
    vc -- vd -- ve -- vc;
    vb -- vc;
}
```

which can be transformed by running `dot -Tpng hello.dot >hello.png` which
yields [hello.png](hello.png).

![hello.png](hello.png)
