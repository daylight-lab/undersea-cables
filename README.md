# undersea cables

Analyzing a network (graph) of undersea cable connectivity.

# use

To use our data, download one of the `.networkx` files and use [NetworkX's `read_gpickle`](https://networkx.org/documentation/stable/reference/readwrite/generated/networkx.readwrite.gpickle.read_gpickle.html#networkx.readwrite.gpickle.read_gpickle) method.

- `_today.network` describes the network today.
- `_future.network` describes the network when all planned projects are fully operational.

NOTE: Networks are bidirectional graphs rather than MultiGraphs (i.e., even if a country has multiple connections to another, there will only be one edge between them). This allows us to compuete betweenness centrality. But you can easily construct a MultiGraph if you want to.

# develop

Clone this repo, and in it, do:

```
python3 -m venv venv
source venv/bin/activate
pip3 install -r requirements.txt
jupyter notebook
```


# license

bsd
