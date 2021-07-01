# OpenAnnotationIO
## Abstract
Traditional annotations are marginalia, errata, and highlights in printed books, schemas, picture, and other physical media. Open Annotations are an attempt to recreate and extend that functionality as a new layer of interactivity and linking on top of the fabric of reality. 

It will allow anyone to annotate anything anywhere, be it a pdf, an timeline, a video, an image, a 3d model, an audio stream, or data in raw or visualized form. Open Annotations can be linked, shared between services, tracked back to their origins, searched and discovered, and stored wherever the author wishes; the vision is for a decentralized and open annotation infrastructure.

## Introduction
Annotating, the act of creating associations between distinct pieces of information, is a driving activity of any creative and technical process, but currently lacks a uniform approach. 

The interactive and collaborative world we live in, where citizens are part of a global community, has produced an environment that both socially motivate and give rise to technical challenges for annotating.

Currently, comments are made using tools built in to various systems. In addition to commenting on resources in a wide variety of social media and creative platforms, there are a plethora of closed and proprietary web-based "sticky note" systems and stand-alone multimedia annotation systems.

The primary downfall about these types of systems is that the user-created annotations cannot be shared or reused due to a deliberate "lock-in" strategy within the environments where they were created. The basic requirement is a common approach to model and express annotations. 

This is the primary aim of OpenAnnotationIO.

OpenAnnotationIO aim to provide a simple extendable way to share and model complex annotation networks while remaining simple enough to be used in the most common use cases, like attaching a piece of text to a single media.

The intended use of OpenAnnotatioIO interoperability is either for sharing public annotations with others or for the migration of private annotations between systems or devices. The annotations must be able to be integrated into existing media collections, APIs, metadata storages and reused without loss of significant information, retaining the contextuality.

## Guiding Principles and Values
The primary aim is to create a standard description framework for sharing annotations between systems.

## Basics
### Annotation 
An Annotation is a Resource. An Annotation usually has a single Body, which is a comment, a scribble, a video an image a sound, and a Target that the Body is somehow "about". The Annotation could contain also additional descriptive properties.

**Example Use Case**: Gaelle has written a note that makes a comment about a particular movie shot. Her client application creates an Annotation with the note as the body resource, and the movie shot as the target resource.

### Motivations
The “aboutness” that is described in the Annotation is conveyed using an instance of the oaio:Motivation class.

## Use Cases

## Data Model

## Data Model Modules

## Interoperability

### OTIO

### USD

### EXR Metadata

### QuickTime Metadata


