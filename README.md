# OpenApp.js

## charter

to create a next-generation, truly modular (built from [node.js modules](http://npmjs.org)), full-stack javascript framework that interoperates with the [Open App Ecosystem](https://github.com/open-app/core).

## feature requirements

- resources are commonly understood entities (Linked Data vocabularies)
- holons (people and recursive groups) are identities
- identities are cryptographic keys
- each holon has a unique primary data service
- each service can be many micro data services
- services can have many different interfaces (HTTP, WebSockets, [jschan](https://github.com/GraftJS/jschan), command-line, ...)
- services describe their interfaces through hypermedia ([JSON-Schema](http://json-schema.org/), [Hydra](http://www.hydra-cg.com/), [JSON-API](http://jsonapi.org/), ...)
- each primary data service can have many cached replicas
- primary data services publish changes to subscribed cached replicas
- cached replicas provide pipeline to submit changes to primary data services
- trust relationships between identities determine cross-service network topology
- resources transfer through services across trust relationships (CPU cycles, data storage, food, shelter, ...)
- transfer between services can employ many different patterns of conversation (request / response, publish / subscribe, push / pull, even more complex patterns like conversations of action)
- data services store transactions on state instead of state
- data services employ conflict resolution algorithms on transactions
- data is immutable and flows instead of changes (consequence of all the above)
- data is validatable (with hashes or signatures)
- data is securable (with encryption)
- data services are de-coupled from views
- views are composable, [one-directional](https://raynos.github.io/forwardjs2014-talk/) components
- generic views can be generated from data and relevant hypermedia

## sub ecosystems

- [mercury](https://github.com/Raynos/mercury)
- [leveldb](http://leveldb.org/)
- [secure-scuttlebutt](https://github.com/dominictarr/secure-scuttlebutt)
- [jshttp](https://jshttp.github.io/)
- [pillarjs](https://github.com/pillarjs)
- [graft](https://github.com/graftjs/graft)
- [node-organic](http://node-organic.com)

and more
