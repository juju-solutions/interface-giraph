# Overview

This interface layer handles the communication between Apache Giraph and
its clients.


# Usage

## Provides

Charms providing this interface need the Apache Giraph.

This interface layer will set the following states, as appropriate:

  * `{relation_name}.joined`   The relation to Giraph has been initialized.


## Requires

Charms requiring this interface make Apache Giraph available.

This interface layer will set the following state, as appropriate:

  * `{relation_name}.joined`   The relation to Giraph has been initialized.

An example use might be:

```python
@when('giraph.joined')
def giraph_joined(giraph):
    .....
```

# Contact Information

- <bigdata@lists.ubuntu.com>
