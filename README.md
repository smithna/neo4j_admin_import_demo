# Neo4j-admin import demo
The notebook in this repo demonstrates how to use the `neo4j-admin import` tool
to load data from CSV into Neo4j.

The example was created with Neo4j 5.8 running in Neo4j desktop on a 
Mac operating system. Some modification to the code might be necessary
to execute the commands in a different environment. Consult the
[documentation](https://neo4j.com/docs/operations-manual/current/tools/neo4j-admin/neo4j-admin-import/)
for the latest information on how to use the bulk importer.

This example demonstrates both a full import, which requires
starting from a blank database, and an incremental import, which allows
you to add new data to an existing database.

Note the [usage and limiatations](https://neo4j.com/docs/operations-manual/current/tools/neo4j-admin/neo4j-admin-import/#_usage_and_limitations)
section of the documentation for the incremental import command. This tool can only
be used to add new nodes and new relationships. *It cannot update or delete properties, 
nodes, or relationships.*