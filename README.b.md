<img src="diagrams/ThinkTank.svg" width="280" />

# Metadata Serialization

This document offers ways for platforms that are part of the NIH Data Commons Pilot to demonstrate Key Capability 7 (KC7), which is needed to guarantee the findability and portability of data. This document was prepared for Team Calcium. Examples and links from existing platforms will be added as they become available.

If you know of useful Metadata Serialization techniques please make a Pull Request!

1. [Metadata Portability](#portability)
2. [Concepts](#concepts)
3. [Use Cases](#usecases)
4. [Core Metadata](#coremetadata)
5. [Ontology Services](#services)
6. [schema.org](#schema)
7. [Case Studies](#casestudies)

<a name="portability" />

## Metadata Portability

Not transferring all the data, just metadata.

<a name="concepts" />

## Concepts

### Data 

For the purposes of this document it is important to separate the concepts of
data from metadata. Data are the first order items one would like to share, 
for example, a VCF might be data, while the file checksum would be metadata.

### Metadata

Metadata describe data and are usually string keys paired with string, numeric, 
array, or object-like values. Metadata should be representable in JSON schemas.

### Data Object

A file, resource, or API that has been uniquely identified for a given 
service, and which provides a minimum of fields from the Data Object 
Service schema.

### Serialization

### JSON

JavaScript Object Notation is a scheme for transmitting data between web 
services. Both metadata and interface methods for services in this document
communicate using JSON.

### JSON-LD

Extensions to JSON that allows it to represent links between Objects using
the addition of @context and @id protected keys.

### Ontology

A controlled vocabulary that allows hierarchical relationships between items
to be represented in a machine readable way.

### API

Application Programming Interface allow applications to be extended to other 
purposes and for programs to more easily communicate with each other.

### Extract

The process of accessing the relevant APIs needed to select some metadata for 
export. This can be carried out by one or more programs and often requires 
performing authenticated requests against a platform. The first stage of the
Extract, Transform, Load process.

### Transform

Data extracted from a platform is altered into a format suitable 
for loading into another platform. Explicit assumptions about the data model 
of the target format are made clear in transformer programs. The second 
stage of the Extract, Transform, Load process.

### Load

Once data have been tranformed into a format that is suitable for indexing 
into a platform, loader programs call the required submission APIs. The last 
stage of the Extract, Tranform, Load process.

<a name="usecases" />

## Use Cases

### Export Metadata to a Serialization Format

### Import Metadata from a Serialization Format

### Export and Import Using the Same Format

<img src="diagrams/exporter-importer.svg" />

### Export Metadata from Platform A and Import to B

<img src="diagrams/exporter.svg" />

### Transformer Detail

<img src="diagrams/transformer.svg" width="425" />


<a name="coremetadata" />

## Core Metadata

The metadata required to represent Data Objects.

<a name="schema" />

## schema.org

schema.org

<a name="services" />

## Ontology Services

Services that provide useful JSON-LD context.

<a name="casestudies" />

## Case Studies

