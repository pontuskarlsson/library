# Basic Body Regions

## Overview

Basic Body Regions provides a standardized hierarchy of human body regions using common, everyday terminology. This data library is designed for use in body measurement systems, digital avatars, and apparel applications where clear, consumer-friendly language is essential.

## Purpose

This library serves as the foundational reference for:
- Locating body landmarks for measurement systems
- Defining regions for points of measure (POMs)
- Creating digital avatars with standardized body references
- Apparel design and fitting systems
- Consumer-facing measurement applications

## Structure

The hierarchy is organized into four main regions with a maximum depth of 4 levels:

### Main Regions
- **Head**: Including face, scalp, and ears
- **Neck**: Front, back, and sides
- **Upper Body**: Trunk and arms from shoulders to waist
- **Lower Body**: Everything below the waist

### Key Features
- **Bilateral Regions**: Marked for body parts that exist on both sides (arms, legs, eyes, etc.)
- **Aliases**: Common alternative names included where applicable
- **Clear Descriptions**: Each region includes a description for clarity
- **Practical Depth**: Maximum 4 levels deep for usability

## Usage Example

When defining a landmark:
```json
{
  "name": "Shoulder Point",
  "bodyRegion": {
    "basic": ["Upper Body", "Arm", "Shoulder"]
  }
}
```

When defining a point of measure:
```json
{
  "name": "Waist Circumference",
  "bodyRegion": {
    "basic": ["Upper Body", "Waist"]
  }
}
```

## Related Data

- **Anatomical Body Regions**: Medical terminology version (coming soon)
- **Body Landmarks**: Reference points that use these regions
- **Points of Measure**: Measurement definitions that reference these regions

## Version History

- **1.0.1** (2025-08-12): Version alignment with schema
- **1.0.0** (2025-08-12): Initial release

## Schema Compliance

This data validates against [Body Regions Schema v1.0.1](https://raw.githubusercontent.com/pontuskarlsson/schemas/main/schema-body-regions/manifest.json)

## License

This data is licensed under the Creative Commons Attribution-ShareAlike 4.0 International License.

## Contributing

Contributions are welcome! Please ensure any modifications:
- Maintain the consumer-friendly terminology
- Include clear descriptions
- Follow the established hierarchy pattern
- Validate against the body regions schema

## Maintainer

Maintained by Pontus Karlsson. For questions or contributions, please visit [GitHub](https://github.com/pontuskarlsson/library).