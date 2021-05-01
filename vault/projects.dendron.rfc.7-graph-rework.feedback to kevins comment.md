---
id: 47d2587f-ddda-4ee5-ae25-9d921ee42aac
title: Feedback to Kevins Comment
desc: ''
updated: 1619855979819
created: 1619638627729
---

## Summary

Thank you for your kind feedback.

## Graph Backend

1. Choice of Database:
    * GunDB:
    It can be seen as a synchronization protocol.
    If we see it that way, we can synchronize the information from the backend with the Plugin using Gun.
    * Pouchdb:
    It could be used to store the data in the backend.
2. Data Structure:
    
    * 



Sadly I have not much information about pouchdb, but what I know is that GunDB is more like a Graph synchronization protocol.
So they could even be combined, making PouchDB the store of value and allowing GunDB to connect the different parts of dendron. 
Naturally, this would depend on if a Webview could connect to a Websocket the engine provides.
We are leaving the Plugin out of the scope for refreshing the graph view.

Additionally, even using one of these DBs wouldn't prevent us from adjusting our Datastrucktures to factor in the Graphology spec.
Implementing this spec would allow us to pass the Graph object into the Layout algorithm to render them using d3.

Further more their is a parser and writer for Graphology that turns Graphology graphs into the gram text format [Graphology Gram](https://github.com/gram-data/graphology-gram) which would make it easier to embed the graph.

