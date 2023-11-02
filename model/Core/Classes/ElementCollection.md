SPDX-License-Identifier: Community-Spec-1.0

# ElementCollection

## Summary

A collection of Elements, not necessarily with unifying context.

## Description

An Element Collection is a collection of Elements, not necessarily with unifying context.

Note that all ElementCollections must conform to the core profile even if the core profile is no specified in the profileConformance property.
If the profileConformance property is not provided, core is to be assumed as the default.

## Metadata

- name: ElementCollection
- SubclassOf: Element
- Instantiability: Abstract

## Properties

- element
  - type: Element except NOT (SpdxDocument) (NOTE: the spec generator still needs to define the official syntax and generation algorithm for the "except NOT (SpdxDocument)" portion here)
  - minCount: 1
- rootElement
  - type: Element except NOT (SpdxDocument) (NOTE: the spec generator still needs to define the official syntax and generation algorithm for the "except NOT (SpdxDocument)" portion here)
  - minCount: 1
- profileConformance
  - type: ProfileIdentifierType
