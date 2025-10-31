# Tone Matching App

A participatory phonology analysis tool for native speakers to compare and group words by tone melodies.

## Project Structure

This repository contains three main components:

### 1. Mobile App (`mobile_app/`)
A Flutter application for Android and Windows Desktop that allows native speakers to:
- Load phonological data bundles
- Compare words and group them by tone melody
- Capture exemplar images for each tone group
- Export results with tone group assignments

### 2. Bundler App (`bundler_app/`)
An Electron desktop application for researchers to:
- Configure phonological data bundles
- Select Dekereke XML files and audio files
- Define display settings and data mappings
- Generate bundle zip files for the mobile app

### 3. Comparison App (`comparison_app/`)
An Electron desktop application for researchers to:
- Import results from multiple native speakers
- Compare tone groupings across speakers
- Identify disagreements and overlaps
- Merge and reconcile tone group classifications

## Requirements

- **Mobile App**: Flutter SDK 3.0+, Dart 3.0+
- **Desktop Apps**: Node.js 18+, npm

## Getting Started

### Mobile App
```bash
cd mobile_app
flutter pub get
flutter run
```

### Bundler App
```bash
cd bundler_app
npm install
npm start
```

### Comparison App
```bash
cd comparison_app
npm install
npm start
```

## Workflow

1. **Researcher prepares data**: Use the Bundler App to create a data bundle from Dekereke XML files and audio files
2. **Native speaker analysis**: Load the bundle in the Mobile App and group words by tone melody
3. **Export results**: Mobile App exports modified XML, CSV summary, and exemplar images
4. **Compare results** (optional): Use the Comparison App to analyze results from multiple speakers

## License

Copyright (c) 2025. All rights reserved.
