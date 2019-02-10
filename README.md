Based on cothority_template (https://github.com/dedis/cothority_template).

The protocol leader, i.e., the tree root, sends announcements down the tree. When receiving an announcement, every node generates a random number. Tree leaves start sending their random numbers back to the leader up the tree, intermediate nodes filter out the smaller numbers, and eventually the root will have the highest number with the node ID that generated it.
