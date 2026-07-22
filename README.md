# GDM-USQRL

**Gana.DM Universal Standard for Quick Reference Libraries**

**A semantic knowledge organization and markup language.**

*Standardizing the way knowledge is organized.*

---

## What is GDM-USQRL?

**GDM-USQRL (Gana.DM Universal Standard for Quick Reference Libraries)** is a semantic knowledge organization and markup language.

Its purpose is to establish a standard for structuring information consistently, allowing different areas of knowledge to be organized following the same logic.

Instead of describing how information should be visually presented, GDM-USQRL describes the **meaning and organization** of knowledge, making it predictable, reusable, and independent from any specific application.

---

## The Problem

Knowledge can be acquired, reviewed, and expanded throughout a person's entire life.

However, the way knowledge is organized usually varies according to the tools used, the author, or the moment when it was created.

Text documents, notes, wikis, and other formats allow information to be recorded, but they usually do not establish a common organizational standard.

As a result, each collection of content develops its own structure, making it harder to locate specific information, review previously studied topics, and reuse accumulated knowledge over time.

As the amount of information grows, remembering where specific knowledge was stored becomes increasingly difficult.

The knowledge still exists, but finding it often depends on the memory of the person who organized it.

---

## The Solution

GDM-USQRL proposes a different approach to knowledge organization: instead of standardizing knowledge itself, it standardizes the way knowledge is organized.

By defining a consistent semantic organization, documents from different areas of knowledge can share the same structural logic.

This makes information retrieval more predictable, facilitates review, and reduces dependence on remembering how each collection was organized.

With a common structure, users learn the pattern once and can apply it to any compatible library, regardless of its subject.

---

## Language Philosophy

GDM-USQRL is based on the fundamental principle of separating knowledge from presentation.

The language does not define how information should be displayed, but how it should be organized and semantically identified.

The responsibility for presentation belongs to the tools that interpret the language.

The goal of GDM-USQRL is not to replace existing knowledge, but to create a structure that allows knowledge to be organized consistently, making consultation, review, and expansion more efficient over time.

> **GDM-USQRL does not standardize knowledge; it standardizes the way knowledge is organized.**

Organizational standardization works as a location system.

Just as a person knows where to find a key because they always place it in the same location, users of GDM-USQRL know where to look for information because it follows a known structure.

The value of the language is the predictability of organization, allowing knowledge to remain accessible even after long periods of time.

---

## Features

### Semantic Organization

GDM-USQRL organizes information based on the meaning of each element, allowing knowledge to be structured clearly and consistently.

### Presentation Independence

The language describes the structure of knowledge, not its visual appearance.

Different tools can interpret the same information in different ways.

### Domain Independence

GDM-USQRL can organize knowledge from different areas without depending on a specific subject.

Examples:

- Programming
- Philosophy
- Mathematics
- History
- Medicine
- Cooking
- Technical documentation

### Standardized Structure

Documents created using the language follow a common organization, making knowledge easier to locate, review, and reuse.

### Extensibility

The language can evolve and receive new elements and features without losing its fundamental principles.

### Compatibility

Different tools can create, interpret, and validate content compatible with the standard.

### Long-Term Organization

GDM-USQRL is designed for knowledge that may be revisited years later, maintaining a clear and understandable structure over time.

---

## Use Cases

GDM-USQRL can be used to organize any type of knowledge that requires a consistent, searchable, and reusable structure.

### Education

Creation of study materials, courses, guides, and educational knowledge bases.

Examples:

- Lessons
- Summaries
- Concepts
- Exercises
- References

---

### Personal Research and Study

Creation of personal knowledge organization systems.

Examples:

- Study notes
- Research
- Reviews
- Future references

---

### Technical Documentation

Organization of structured technical knowledge and documentation.

Examples:

- Software documentation
- Manuals
- Guides
- References
- Procedures

---

### Specialized Knowledge

Organization of knowledge from specific fields.

Examples:

- Philosophy
- History
- Medicine
- Law
- Engineering
- Cooking

---

### Creative Projects

Organization of complex fictional and creative information.

Examples:

- RPG worlds
- Worldbuilding
- Narratives
- Fictional encyclopedias

---

## Ecosystem

GDM-USQRL is the foundation of an ecosystem of tools and formats designed to work with structured knowledge.

The language defines how knowledge is organized semantically. Other components can be developed to store, distribute, edit, validate, and interpret this knowledge.

```
GDM-USQRL
     │
     ▼
Compatible formats and libraries
     │
     ▼
Interpretation and usage tools
```

GDM-USQRL does not depend on a specific application.

Any compatible tool can use the language by following this specification.

Gana.DM is one of the first implementations created to interpret and use GDM-USQRL content, but the language remains independent from any individual application.

---

## Simple Example

A GDM-USQRL document is composed of elements that represent parts of knowledge.

These elements describe the structure and meaning of information, allowing different types of content to use the same organization model.

Example:

```json
{
  "content": [
    {
      "type": "title",
      "text": "Chocolate Cake"
    },
    {
      "type": "description",
      "text": "A simple chocolate cake recipe."
    },
    {
      "type": "list",
      "title": "Ingredients",
      "items": [
        "Flour",
        "Chocolate",
        "Eggs",
        "Milk"
      ]
    },
    {
      "type": "list",
      "title": "Preparation",
      "items": [
        "Mix the ingredients",
        "Prepare the dough",
        "Bake the cake"
      ]
    }
  ]
}
```

In this example, GDM-USQRL does not define the visual appearance of the recipe.

It only defines that the document contains:

- a title;
- a description;
- organized groups of information.

The same structure could be used for different areas of knowledge.

The meaning comes from the content, while the organization remains standardized.

---

## Project Goals

The goal of GDM-USQRL is to create an open standard for semantic knowledge organization and markup, allowing information to be structured, shared, and reused consistently.

Long-term goals include:

- Creating a universal way to organize knowledge.
- Allowing different fields to use a common structure.
- Facilitating review and reuse of information over time.
- Separating knowledge meaning from presentation.
- Encouraging the creation of compatible tools.
- Building an open ecosystem based on a shared language.

---

## Project Status

GDM-USQRL is currently in the development and specification definition phase.

Current work focuses on:

- defining the principles of the language;
- organizing the document model;
- defining semantic elements;
- creating validation rules;
- developing JSON Schema support;
- documenting the specification.

The specification is still evolving.

Future decisions may expand the language while preserving its fundamental principles:

- semantic organization;
- presentation independence;
- standardized knowledge structure.

---

## Documentation

The GDM-USQRL documentation is divided into different levels to serve different needs.

### Introduction

Presents the proposal, philosophy, and goals of the language.

### Specification

Defines the technical rules of GDM-USQRL, including:

- document structure;
- language elements;
- properties;
- validation rules;
- version compatibility.

### Schema

Contains validation files used to assist in the creation of compatible documents.

### Examples

Contains demonstration documents and examples to help understand the language.

---

## License

GDM-USQRL is an open specification project.

The use, implementation, and creation of compatible tools are encouraged according to the project's license terms.

The official license will be defined during the publication of the project.