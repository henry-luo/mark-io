# mark-io
A light framework for converting anything into Mark, and convert Mack back to anything. (alpha)

This project is still in early brain-storming stage.

### Why mark-io?
Unlike other widely adopted data formats, like JSON, XML, HTML, which aleady have a lot data to work with, there's almost no data in Mark at the moment. Thus we need this project to bridge the gaps between Mark and rest of the world.

### Why a framework?
Becasue it will more than just a bunch of library code, there'll be conventions/structures/options for doing things, thus a framework.

But we don't want it to be too restrictive, too strong opinioned. So it should be a *light* framework for people to further build useful things on top of it.

## Architecture
- scope of mark-io:
  - anything => mark, mark => anything;
- design:
  - a modular and plugin-based approach:
    - parsers and serializers: generic grammar-based parsers to convert text sources into Mark;
    - adaptors: for working with binary data;
    - connectors: for connecting to various data sources, like RDB, FS, REST;
  - so what unifies all these data formats/sources, is not the Mark syntax, but the Mark data model!
- integration with other projects:
  - transformation, i.e. mark => mark, will be done in mark-template;
  - schema validation, will be done in mark-schema;
- phases:
  - phase 1: DOM/AST based;
  - phase 2: stream based;



