# Portolan Data

This repository coordinates official Portolan catalogs and community mirrors.
Each issue tracks one dataset from proposal through publication.

A Portolan catalog publishes geospatial data as plain files in cloud storage.
People and agents can inspect the metadata and query the data with standard tools.
The [Portolan registry](https://github.com/portolan-sdi/portolan-registry) connects published catalogs into a searchable network.

## Propose a Dataset

Use the [dataset proposal form](https://github.com/portolan-sdi/portolan-data/issues/new?template=dataset_request.yml) to suggest a dataset.
You only need information about the source and why the dataset would be useful.

The form asks for:

- The dataset name and publisher.
- The upstream source URL.
- The license or terms, if known.
- The reason the dataset would be useful in Portolan.
- Optional notes about coverage, formats, update frequency, or access constraints.

You do not need to design the catalog or plan the conversion work.

## How Accepted Datasets Are Published

When Portolan accepts a proposal, contributors:

1. Mirror the source data.
2. Convert the data to Portolan-supported cloud-native formats where needed.
3. Publish the data and metadata as a Portolan catalog.
4. Submit the catalog to the [Portolan registry](https://github.com/portolan-sdi/portolan-registry).

The [Portolan spec](https://github.com/portolan-sdi/portolan-spec) defines the catalog requirements.
The [Portolan CLI](https://github.com/portolan-sdi/portolan-cli) supports catalog creation.

## Official Catalogs and Mirrors

An official catalog comes from the organization that publishes the dataset.
A mirror republishes an upstream dataset as a Portolan catalog.

Mirrors keep the source visible in their metadata.
They use a `via` link for an upstream source or a `canonical` link for an upstream STAC catalog.
They also record the date of the latest mirror update.

## Contribute a Catalog

To work on an accepted proposal, comment on its issue before you start.
This helps contributors avoid duplicate work and coordinate open questions.

You can host a catalog in your own S3-compatible storage.
[Source Cooperative](https://source.coop/) also provides free storage for open data.
The shared Portolan mirrors organization is available for suitable community mirrors.
See [portolan-ops#1](https://github.com/portolan-sdi/portolan-ops/issues/1) for current hosting details.

For questions, use the [Portolan Google Group](https://groups.google.com/g/portolan) or the [Portolan channel](https://cloudnativegeo.slack.com/archives/C0A1JBH9529) in Cloud-Native Geo Slack.

Portolan is an open-source standard under the Apache-2.0 license.
Visit the [Portolan website](https://www.portolan-sdi.org/) for the overview and documentation.
