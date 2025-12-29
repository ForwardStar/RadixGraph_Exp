# RadixGraph_Docker

Reproduce RadixGraph experimental results using Docker.

# Build the minimal Docker image

This image only tests the LiveJournal dataset experiments.

```bash
docker build -f Dockerfile_minimal -t radixgraph:minimal .
```

# Build the full Docker image

This image includes all datasets and experiments. It might take days to finish.

```bash
docker build -f Dockerfile_full -t radixgraph:full .
```

# Run whichever image you want
```bash
docker run -it radixgraph:minimal
```

or:
```bash
docker run -it radixgraph:full
```