# GDM-USQRL

## Gana.dm Universal Standard for Quick Reference Libraries

> 🇧🇷 Usuários brasileiros: uma versão traduzida deste README está disponível em [Português Brasileiro](translations/pt-br/README.md).

---

# About

GDM-USQRL is a data organization specification based on JSON files for creating quick reference libraries.

The specification defines a standardized structure for organizing information in a simple, consistent, and accessible way.

It is not an application, program, language, or platform. It is a data structuring convention that defines how JSON files can be organized to represent quick reference libraries.

---

# Objective

The structure was created to facilitate the storage, organization, and retrieval of information.

The objective is to allow different types of knowledge to be organized using a common model.

The structure enables:

- Consistent organization of information.
- Quick access to specific content.
- Separation between organization and data.
- Human and application-readable information.
- Data reuse across different projects.

---

# Applications

The specification is not limited to a specific area.

It can be used to create libraries for any type of knowledge, including:

- Technical documentation.
- Personal studies.
- Educational materials.
- Sciences.
- History.
- Languages.
- Professional references.
- Information collections.
- Programming and technology.
- Any other organized set of knowledge.

The purpose of each library depends on the objective of its creator.

---

# Concept

A quick reference library organizes information so that specific content can be found efficiently.

The structure uses a separation between:

- Indexes, responsible for organization and navigation.
- Storage, responsible for individual content.

This separation allows large collections of information to be organized without depending on a single file containing all data.

---

# General Structure

A library follows a hierarchical organization:

```text
Library

├── Indexes

└── Contents
```

The relationship between data follows:

```text
Library

↓

Groups

↓

Individual items
```

---

# File Architecture

Example of organization:

```text
library/

├── index.json

├── groups/

│   ├── group-1.json

│   ├── group-2.json

│   └── group-3.json

└── storage/

    └── library-name/

        ├── group-name/

        │   ├── item-001.json

        │   ├── item-002.json

        │   └── item-003.json
```

---

# Index

The main `index.json` file contains general information about the library.

It can define:

- Library identification.
- General information.
- Group locations.
- Main structural relationships.

---

# Groups

Groups represent internal divisions used to organize related content.

They work as intermediate indexes between the library and individual items.

Example:

```text
Library

├── Group A

├── Group B

└── Group C
```

Each group contains information that allows its respective items to be located and organized.

---

# Storage

The `storage` directory contains individual files with the complete content of each item.

The organization follows:

```text
storage/

└── library/

    └── group/

        └── item.json
```

Each file represents an independent unit of information.

---

# Items

Items represent the smallest unit of information within the structure.

An item can represent any type of content:

- Concept.
- Reference.
- Definition.
- Element.
- Command.
- Specific information.
- Knowledge record.

Example:

```json
{
  "id": "example-item",
  "title": "Item title",
  "subtitle": "Additional information",
  "description": "Content description."
}
```

---

# Separation Between Structure and Content

The organization separates two main parts.

## Structure

Responsible for:

- Indexes.
- Groups.
- References.
- File paths.
- Library organization.

## Content

Responsible for:

- Titles.
- Descriptions.
- Examples.
- Specific item information.

This separation allows different applications to use the same data.

---

# Technical Data and Natural Content

The files contain information intended for different purposes.

## Technical Data

Used for identification, reference, and organization.

Example:

```json
{
  "id": "example-item"
}
```

## Natural Content

Used to present information in a way that is understandable to people.

Example:

```json
{
  "title": "Item title",
  "description": "Content description."
}
```

Technical fields follow a structure defined by the specification.

Textual content can be written in the language chosen by the library creator.

---

# Language

The specification does not define a mandatory language.

Each library can use the language most appropriate for its purpose, audience, or context.

A library can be:

- Personal.
- Internal to a project.
- Public.
- Intended for a specific community.
- Multilingual when necessary.

Creating translations is optional.

The universality comes from the data structure, not from the language used.

---

# Compatibility

Any application capable of interpreting JSON files according to the defined structure can use a compatible library.

The specification allows different implementations without depending on a specific application.

---

# License

GDM-USQRL is an open specification for organizing quick reference libraries using JSON files.