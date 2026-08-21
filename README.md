# Portolan Data

This repository supports the open-source Portolan community.
Contributors use it to coordinate official Portolan catalogs and community mirrors.

A Portolan catalog publishes geospatial data as plain files in cloud storage.
People and agents can inspect the metadata and query the data with standard tools.
The [Portolan registry](https://github.com/portolan-sdi/portolan-registry) connects published catalogs into a searchable network.

## Propose a Dataset

If you publish or maintain a dataset, build a Portolan catalog and submit it to the [Portolan registry](https://github.com/portolan-sdi/portolan-registry).
Community contributions do not need a proposal here first.

Use the [dataset proposal form](https://github.com/portolan-sdi/portolan-data/issues/new?template=dataset_request.yml) for datasets that need community attention.
The form is especially useful for a global dataset with broad public value.
The proposal gives contributors a place to coordinate the work.

The form asks for:

- The dataset name and publisher.
- The upstream source URL.
- The license or terms, if known.
- The reason the dataset would be useful in Portolan.
- Optional notes about coverage, formats, update frequency, or access constraints.

You do not need to design the catalog or plan the conversion work.

## How the Community Publishes Proposed Datasets

When contributors take on a proposal, they:

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

Build a catalog for a dataset you publish, maintain, or want to mirror.
Submit the catalog to the [Portolan registry](https://github.com/portolan-sdi/portolan-registry) when it meets the spec.

To work on a proposal from this repository, comment on its issue before you start.
This helps the community avoid duplicate work and coordinate open questions.

You can host a catalog in your own S3-compatible storage.
[Source Cooperative](https://source.coop/) provides free hosting for data that supports the Portolan project.
The shared Portolan mirrors organization is available for suitable community mirrors.
See [portolan-ops#1](https://github.com/portolan-sdi/portolan-ops/issues/1) for current hosting details.

For questions, use the [Portolan Google Group](https://groups.google.com/g/portolan) or the [Portolan channel](https://cloudnativegeo.slack.com/archives/C0A1JBH9529) in Cloud-Native Geo Slack.

Portolan is an open-source standard under the Apache-2.0 license.
Visit the [Portolan website](https://www.portolan-sdi.org/) for the overview and documentation.
