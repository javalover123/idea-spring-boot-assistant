# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com), and this project adheres
to [Semantic Versioning](https://semver.org).

## [Unreleased]

### Added

- Inspection: Report deprecated properties.
- Join lines will join keys in yaml.
- Support
  for [value providers](https://docs.spring.io/spring-boot/docs/current/reference/html/configuration-metadata.html#configuration-metadata.manual-hints.value-providers)

### Changed

### Deprecated

### Removed

### Fixed

### Security

## [0.15.0] - 2022-10-17

### Added

- Inspection: Report undefined properties.
- Inspection: Report invalid property values.

## [0.14.5] - 2022-10-06

### Removed

- If there is bundled Spring Framework support, this plugin will be disabled(the bundled Spring support is good enough),
  that means IntelliJ IDEA Ultimate is not supported.

### Fixed

- Compatibility improvements.

## [0.14.4] - 2022-10-05
### Added
- [#37](https://github.com/flikas/idea-spring-boot-assistant/pull/37) - Support `bootstrap.yaml` by default. (by
  guchengod)

## [0.14.3] - 2022-06-04
### Fixed
- [#15](https://github.com/flikas/idea-spring-boot-assistant/issues/15) - File not found rarely when reading user
  defined spring-configuration-metadata file.
- [#16](https://github.com/flikas/idea-spring-boot-assistant/issues/16) - Cannot get element's document when editing
  yaml file which is exists only in memory.

## [0.14.0] - 2022-05-21
### Added
- Intelligence insert in yaml file: Add new property anywhere, insertion will happen at right place.
- Bug reporting: Create issue at GitHub from IDE error dialog.

## [0.13.0] - 2022-05-04
### Added
- Spring yaml properties file have got a new icon.
- 'Go to declaration(Ctrl-B or Ctrl-Click)' will navigate to the source code of the property in yaml properties file.

### Changed
- This plugin will be activated only in application*.yml/yaml files by default, this will avoid some annoying side
  effects while you are editing other yaml files, these settings can be changed at Settings->Editor->File Types->"Spring
  yaml properties file".
- The document of properties is better formatted.

### Fixed
- After rebuild, generated metadata files in project is not correctly reindex-ed.
- 'additional-spring-configuration-metadata.json' file has not been correctly processed sometimes.
- Document is missing while @ConfigurationProperties annotated class is using lombok to generate properties.
- "com.intellij.diagnostic.PluginException: same CV with different captured context" while code completion.

## [0.2.2] - 2021-10-20
### Added
- Compatible with IntelliJ IDEA Community Edition 2021.3.

## [0.1.3] - 2021-10-10
### Fixed
- Fixed issue with metadata not updated after maven reimport.

## [0.1.0] - 2021-10-08
### Changed
- This plugin is now compatible with IntelliJ IDEA Community Edition from version 2019.3 to 2021.2.