# Data Modeling Notes

## Requirements

A client has hired you to build an API for managing `zoos` and the `animals` kept at each `zoo`. The API will be use for `zoos` in the _United States of America_, no need to worry about addresses in other countries.

For the `zoos` the client wants to record:

- name.
- address.

For the `animals` the client wants to record:

- name.
- species.
- list of all the zoos where they have resided.

Determine the database tables necessary to track this information.
Label any relationships between table.

## A good Data Model

- captures all the data the stystem needs
- captures only the information the system needs
- reflect reality (logical information that the system needs)
- flexible so it can evolve
- guarantees data integrity
- is dirven by the way we access data

## components

- entites (nouns: zoo, animal, species), like a resource --> tables
- properties --> columns or fields
- relationships --> foreign keys

## workflow

- identify entities
- identify relationships
- identify properties

## relationships

- one to one
- one to many
- many to many (smoke and mirrors)

## Mantras

- every table must have a **Primary Key**
- work on two or three entities at a time
- one to many relationships are modeled using a foreign key
- the foreign key always goes on the 'many' side
- the foreign key column must be the same type as the primary key it references
- many to many are modeled using a tertiary table- 2 foreign keys to link to each many
- the tertiary table could include other columns
