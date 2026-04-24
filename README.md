# Cumulocity Digital Twin Manager

---

## Note: Project Status

> **⚠️ Discontinued Release**
>
> The open-source release of Cumulocity Digital Twin Manager has been discontinued after version 1019.1.2. This decision was made because our customers now benefit from continuous deployment, which enables them to access changes much faster.
>
> This repository continues to serve as a community resource for asset definition samples.

---

# Cumulocity Digital Twin Manager - Asset Definitions Samples

## About This Repository

This repository contains **Asset Definition** samples for the Cumulocity Digital Twin Manager. This public repository is open for community contributions of useful and reusable asset definitions.

### What are Asset Definitions?

An **Asset Definition** is a blueprint or template used to create one or multiple assets in the Digital Twin Manager. It defines the structure and properties of an asset after it is created, allowing for consistent asset creation across your organization.

Each asset definition consists of:
- **Property Definitions**: Individual properties or attributes that describe characteristics of the asset
- **Subasset Definitions**: Nested asset structures that allow for hierarchical asset organization

Asset definitions enable standardized, repeatable asset creation and ensure consistency across your digital twin landscape.

## Repository Structure

This repository is organized into three sample directories, each representing different versions of the asset definition format:

### `/samples/` - Original Format
Contains the earliest version of asset definition samples. Use this for legacy systems or reference purposes.

- `sample-asset-model-for-solar-power-plant.json` - Solar power plant asset definition
- `sample-asset-model-for-wind-turbine.json` - Wind turbine asset definition
- `sample-asset-models-for-vaccum-factory` - Vacuum factory asset definitions

### `/samples-v2/` - Updated Format
Contains version 2 of the asset definition samples with improvements and refined structure.

- `sample-asset-model-for-solar-power-plant.json` - Solar power plant asset definition (v2)
- `sample-asset-model-for-wind-turbine.json` - Wind turbine asset definition (v2)
- `sample-asset-models-for-vaccum-factory.json` - Vacuum factory asset definitions (v2)

### `/samples-v3/` - Latest Format (Recommended)
Contains the latest version with updated terminology. **This is the recommended version for new projects.**

**Terminology Updates in v3:**
- `assetModels` → `assetDefinitions`
- `assetProperties` → `propertyDefinitions`

- `sample-asset-model-for-solar-power-plant.json` - Solar power plant asset definition (v3)
- `sample-asset-model-for-wind-turbine.json` - Wind turbine asset definition (v3)
- `sample-asset-models-for-vaccum-factory.json` - Vacuum factory asset definitions (v3)

---

## Getting Started

1. **Browse Existing Samples**: Explore the `/samples-v3/` directory for examples of well-structured asset definitions
2. **Review Documentation**: Each sample directory contains a `README.md` with format-specific details
3. **Understand the Format**: Study existing JSON structures to understand the asset definition format
4. **Plan Your Contribution**: Identify an asset type or domain that would be valuable to the community

---

## Contributing to This Repository

We welcome contributions from the community! Asset definitions for new asset types, industries, and use cases are especially valuable. Follow these guidelines to ensure a smooth contribution process.

### Contribution Guidelines

#### 1. **Before You Start**

- **Check for Duplicates**: Search the repository to ensure your proposed asset definition doesn't already exist
- **Create an Issue** (Optional but Recommended): Open a GitHub issue to describe your proposed asset definition. This allows the community to provide feedback before you invest time in development
- **Review Existing Samples**: Study the samples in `/samples-v3/` to understand the current format and naming conventions

#### 2. **Prepare Your Asset Definition**

- **Use Latest Format**: Base your contribution on the v3 format (`/samples-v3/`) with updated terminology (`assetDefinitions`, `propertyDefinitions`)
- **Follow Naming Conventions**:
  - Use descriptive, lowercase file names with hyphens: `sample-asset-model-for-[asset-type].json`
  - Use clear, meaningful property and field names
  - Include descriptive comments where appropriate
- **Validate JSON**: Ensure your JSON is valid and properly formatted. Use a JSON validator tool to verify
- **Document Your Asset**: Include comments or a description explaining:
  - What the asset represents
  - What properties and subassets it includes
  - Any domain-specific information
  - Use cases or application scenarios

#### 3. **Testing & Validation**

- **Test Your Asset Definition**: Verify that your asset definition can be parsed and used in a Digital Twin Manager environment
- **Check for Consistency**: Ensure property names, types, and structures are consistent with existing samples
- **Validate Against Schema**: If applicable, validate your asset definition against the official asset definition schema

#### 4. **Creating Your Pull Request**

- **Fork the Repository**: Create a fork of this repository in your GitHub account
- **Create a Feature Branch**: Use a descriptive branch name:
  ```
  git checkout -b add/asset-definition-for-[asset-type]
  ```
- **Commit Your Changes**: Write clear, concise commit messages:
  ```
  Add asset definition for [asset type]
  
  - Includes [main properties]
  - Supports [key use cases]
  ```
- **Add to Appropriate Directory**: Place your file in `/samples-v3/` unless you have a specific reason to use a different version
- **Update Directory README** (if applicable): If adding to a directory without a README, consider creating one with a brief description

#### 5. **Pull Request Submission**

When submitting your pull request:

1. **Write a Clear Title**: Describe what asset definition(s) you're adding
   ```
   Add asset definitions for industrial equipment monitoring
   ```

2. **Provide a Description**:
   ```
   ## Description
   Adds asset definitions for common industrial equipment.
   
   ## Included Assets
   - Heavy machinery with vibration monitoring
   - Production line conveyor systems
   - Environmental monitoring sensors
   
   ## Validation
   - JSON validated against standard schema
   - Tested with Cumulocity Digital Twin Manager v1019.1.2
   - Follows v3 format and naming conventions
   ```

3. **Reference Any Related Issues**: Use `Closes #[issue-number]` if applicable

4. **Ensure Files Are Formatted**: 
   - JSON is properly formatted and indented
   - No trailing whitespace
   - UTF-8 encoding

#### 6. **Review Process**

- **Community Review**: Your pull request will be reviewed by maintainers and community members
- **Feedback Loop**: Be responsive to feedback and questions
- **Make Revisions**: Update your pull request based on review comments
- **Merge**: Once approved, your contribution will be merged into the main branch

#### 7. **After Merge**

- **Celebrate**: Your contribution is now part of the public repository!
- **Share**: Feel free to share your contribution with the community
- **Maintain**: Help maintain your contribution by responding to issues or questions about it

### Best Practices

- **Reusability**: Create asset definitions that can be used across different organizations and use cases
- **Documentation**: Include sufficient documentation so others can understand and use your asset definition
- **Consistency**: Follow existing naming conventions and structure patterns
- **Versioning**: If updating an existing asset definition, consider incrementing the version in your contribution description
- **Examples**: Include example usage scenarios or provide context for where this asset definition might be useful

### Code of Conduct

We expect all contributors to be respectful and professional. Please adhere to the following:

- Be respectful to other community members
- Provide constructive feedback
- Focus on the asset definition content, not personal criticism
- Resolve disagreements professionally and respectfully

---

## Support & Questions

- **Issues & Bug Reports**: Use GitHub Issues to report problems with existing asset definitions
- **Discussions**: Start a GitHub Discussion for questions about contributions or asset definition best practices
- **Documentation**: Check the `/samples-v3/README.md` for format-specific documentation

---

## License

This repository is provided under the terms outlined in the [LICENSE](LICENSE) file.

---

## Disclaimer

Please refer to the [DISCLAIMER](DISCLAIMER) file for important information regarding the use of these asset definitions.

---

## Community Contributions

Thank you to all the community members who have contributed asset definitions! Your contributions help make the Digital Twin ecosystem more robust and useful for everyone.
