# example

A repo to store examples

# Graphviz

Graph Visualization Software [graphviz](http://www.graphviz.org/) is pretty
neat.  You can get crazy complicated, or stay simple.

## Basic graphs

## Undirected graphs

Something like [hello.dot](hello.dot) is a basic graph:

```dot
graph G {
    va -- vb;
    vc -- vd -- ve -- vc;
    vb -- vc;
}
```

which can be transformed by running `dot -Tpng hello.dot > hello.png` which
yields [hello.png](hello.png).

![hello.png](hello.png)

### Directed graphs (digraph)

Something like [hello_digraph.dot](hello_digraph.dot) is a basic digraph:

```dot
digraph G {
    va -> vb;
    vc -> vd -> ve -> vc;
    vb -> vc;
}
```

which can be transformed by running `dot -Tpng hello_digraph.dot > hello_digraph.png` which
yields [hello_digraph.png](hello_digraph.png).

![hello_digraph.png](hello_digraph.png)

### Basic attributes

You can change things like the orientation of the graph, or the node shapes.

```dot
digraph G {
    va -> vb;
    vc -> vd -> ve -> vc;
    vb -> vc;
}
```

![hello_digraph.png](hello_digraph.png)
