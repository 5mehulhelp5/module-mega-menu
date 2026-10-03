# Changelog

All notable changes to this extension are documented here. The format
is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/).

## [1.0.19] - 2026-10-03

### Fixed
- The navigation block called a missing `isAnimationEnabled()` helper method and failed with a fatal error. The helper now provides it: animation is on unless Animation Type is set to None.
- Moving a menu item no longer fails: the item path and level are recalculated, child item paths are updated recursively, and positions are reindexed for both the old and the new parent.
- `Block\Menu::getMenuHtml()` renders the menu tree with the storefront menu renderer instead of failing with a type error, and `getMenuData()` returns the configured menu's data (or an empty array) instead of failing with an argument count error.
