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

## Terminology
**IRI** https://datatracker.ietf.org/doc/html/rfc3987

**Resource** An item of interest that MAY be identified by an IRI.

## Guiding Principles and Values
The primary aim is to create a standard description framework for sharing annotations between systems.

## Basics
### Annotation 
An Annotation is a Resource. An Annotation usually has a single Body, which is a comment, a scribble, a video an image a sound, and a Target that the Body is somehow "about". The Annotation could contain also additional descriptive properties.

**Example Use Case**: Gaelle has written a note that makes a comment about a particular movie shot. Her client application creates an Annotation with the note as the body resource, and the movie shot as the target resource.

### Motivations
The “aboutness” that is described in the Annotation is conveyed using an instance of the oaio:Motivation class. 

### Selectors
Annotations refer to part of a media, rather than all of it, as the Target. We call that part of the media a Segment. A Selector is used to describe how to determine the Segment from within the Source media. Multiple Selectors can be given to describe the same Segment in different ways.

**Example Use Case:** Gaelle wants to associate a selection of an image in frame version, with another image on the same frame of another version. She selects both using her client application, and creates the Annotation with a SpecificResource that has a Selector for each of the Body and the Target.

#### Fragment Selector
As the most well understood mechanism for selecting a Segment is to use the fragment part of an IRI defined by the representation's media type, To be clear about which fragment type is being used, the Selector may refer to the specification that defines it. The specification should be accessible by anyone accessing the annotation.

**Example Use Case:** Gaelle wants to associate part of a video as the comment for an animation was created by an artist. She selects the time range within the video and clicks that it is describing the target. Her client appllication then creates the Annotation using a SpecificResource with a FragmentSelector and the describing Motivation. 

#### OTIO Selector
Another common method of selecting elements and content within a resource that supports OTIO, is to use an OTIO selection. OTIO allows a great deal of flexibility when describing the editorial structure to the selected content. Results are not defined for when an OTIO Selector is applied to a representation that does not conform to the edit.

**Example Use Case:** Gaelle selects a clip and writes a note about the whole clip. To refer explicitly to this item, her client application use the OTIO structure to identify it as the target of the Annotation.

#### USD Selector

#### OIIO Selector

#### Data Position Selector

#### SVG Selector

#### Range Selector

## Use Cases
While there are too many use cases to discuss them all in detail, it is useful to hightlight some key scenarios that serve as input to the design process.

The most common use case for annotations is simply attaching a textual comment to an existing media. This could take the form of a commenting system, an overlaid digital sticky-note.

An extension to this scenario is when the body or the target being annotated is not just textual. It could be a video or audio file, for example, which is about an image or data set. Commenters can easily leave video or audio comments and associate it with a specific media with the ability to easily upload from mobile devices or computers with webcams.

The ability to annotate arbitrary media is particularly important in many production use cases, where different media formats, large scale datasets, frames, 3d Models and many others are the topic of discussions.

Tagging resources, either with a simple string or a semantic URI, is also a very common case. For instance tagging a media with a specific Vendor ID, Database ID to then pass it along to other vendorts that would tag the resource with their own IDs.

Machines also create annotations to be consumed by other machines. Image/Video Mining applications can quickly annotate every image or audio, and then build upon those annotations to create relationships between them.

### Annotate a single Image

### Annotate a range in a video

### Annotate a 3D Model

### Annotate two media in compare mode

### Annotate a media layer

### Annotate a clip

### Annotate a track

### Annotate a selection of clips

## Data Model

## Data Model Modules

## Interoperability

### OTIO

### USD

### EXR Metadata

### QuickTime Metadata


