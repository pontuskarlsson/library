# Library

## Overview

Open-source data libraries for standardizing body measurements, business entities, and other structured data across industries. All data in this repository follows schemas defined in the [schemas repository](https://github.com/pontuskarlsson/schemas).

## Purpose

This repository provides standardized, version-controlled data libraries that enable:
- Consistent body measurement systems across apparel and avatar platforms
- Standardized business entity definitions
- Interoperable data exchange between systems
- Community-driven improvements and extensions

## Structure

```
library/
├── body-measurements/     # Body measurement foundations
│   ├── body-regions-basic/
│   ├── body-regions-anatomical/
│   ├── body-landmarks/
│   ├── body-points-of-measure/
│   └── body-shapes/
│
├── business/             # Business entity definitions (future)
│   └── ...
│
└── colors/               # Color standards (future)
    └── ...
```

## Body Measurements

The body measurements libraries provide foundational data for:

### Available Libraries

- **body-regions-basic** - Common terminology for body regions (Head, Neck, Upper Body, Lower Body)
- **body-regions-anatomical** - Medical/technical terminology (coming soon)
- **body-landmarks** - Fixed anatomical reference points (coming soon)
- **body-points-of-measure** - Standardized measurement definitions (coming soon)
- **body-shapes** - Body shape classifications (coming soon)

### Use Cases

- Digital avatar creation
- Apparel sizing and fit
- 3D body scanning
- Medical and health applications
- Custom clothing manufacturing
- Virtual try-on systems

## How to Use

### 1. Reference a Library

Each library provides versioned data files that can be referenced directly:

```json
{
  "bodyRegions": "https://raw.githubusercontent.com/pontuskarlsson/library/main/body-measurements/body-regions-basic/versions/1.0.1/data.json"
}
```

### 2. Validate Your Data

All libraries follow schemas from the [schemas repository](https://github.com/pontuskarlsson/schemas):

```json
{
  "$schema": "https://raw.githubusercontent.com/pontuskarlsson/schemas/main/schema-body-regions/versions/1.0.1/schema.json",
  "metadata": {...},
  "regions": {...}
}
```

### 3. Version Management

Each library includes a `manifest.json` with version history:
- Semantic versioning (MAJOR.MINOR.PATCH)
- Change logs for each version
- IPFS support for immutable references
- Breaking change notifications

## Contributing

We welcome contributions! To add or improve a library:

1. **Follow the Schema**: Ensure your data validates against the appropriate schema
2. **Maintain Quality**: Include clear descriptions and documentation
3. **Version Properly**: Follow semantic versioning principles
4. **Test Thoroughly**: Validate your data before submitting
5. **Document Changes**: Update manifest and changelog

See [CONTRIBUTING.md](CONTRIBUTING.md) for detailed guidelines.

## License

All libraries are licensed under [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/). This means:
- ✅ Free to use commercially
- ✅ Can modify and extend
- ✅ Must give attribution
- ✅ Must share under same license

## Related Projects

- [Schemas](https://github.com/pontuskarlsson/schemas) - Schema definitions these libraries follow
- [Body Profile Tools](https://github.com/pontuskarlsson/body-profile-tools) - Tools for working with body measurements (future)

## Roadmap

### Current Focus
- ✅ Basic body regions
- 🚧 Anatomical body regions
- 🚧 Body landmarks
- 🚧 Points of measure
- 📋 Body shapes

### Future Additions
- Business entity types
- Industry classifications
- Color standards
- Material specifications
- Size charts

## Community

- **Issues**: Report problems or suggest improvements via [GitHub Issues](https://github.com/pontuskarlsson/library/issues)
- **Discussions**: Join conversations in [GitHub Discussions](https://github.com/pontuskarlsson/library/discussions)
- **Updates**: Watch this repository for new releases

## Maintainer

Maintained by [Pontus Karlsson](https://github.com/pontuskarlsson). For questions, please open an issue or start a discussion.

---

*Building open standards for a more interoperable future.*