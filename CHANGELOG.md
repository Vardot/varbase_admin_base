# Changelog

All notable changes to the Varbase Admin Base recipe are documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [1.0.0-rc4] - 2026-09-02
### Fixed
- Remove the empty `metatag_display_extender` stanza from `config/views.view.content.yml`
  and `config/views.view.user_admin_people.yml`. Both stanzas carried no data
  (`metatags: {}`, `tokenize: false`), and the extender is provided by the
  `metatag_views` submodule this recipe does not require, so building either admin view
  on a Drupal CMS base fatalled with `PluginNotFoundException`.
### Changed
- Pin the `drupal/varbase_recipes` dependency to `~1.0.0` for the release.
- Update the version badge to `1.0.0-rc4` in `README.md`.

## [1.0.0-rc3] - 2026-09-02
### Added
- Require the `vardot/jquery.fancytree` library (`^2.38.5`), so the recipe brings the
  Fancytree library `drupal/taxonomy_manager` loads from
  `/libraries/jquery.fancytree/dist/`. The suggested `fancytree/fancytree` package does
  not exist on Packagist, so the library never arrived over Composer.
### Fixed
- Install `smart_date` early: it arrives last in the recipe chain and can deadlock a
  Drupal CMS install.
- Fix the `drupal/smart_date` constraint to `~4.3.0`.
### Changed
- Pin the `drupal/varbase_recipes` dependency to `~1.0.0` for the release.
- Update the version badge to `1.0.0-rc3` in `README.md`.

## [1.0.0-rc2] - 2026-09-01
### Added
- Install the Canvas Icon Picker (`drupal/canvas_icon_picker`) beside `ui_icons`, and
  set `allowed_packs` to `bootstrap_icons` and `vartheme_social`, so every Varbase site
  template inherits the searchable, visual icon picker in the Drupal Canvas editor
  instead of a plain select list of icon names.
### Changed
- Pin the `drupal/varbase_recipes` dependency to `~1.0.0` for the release.
- Update the version badge to `1.0.0-rc2` in `README.md`.

## [1.0.0-rc1] - 2026-08-15
### Changed
- Release the recipe with the Varbase 11.0.0-rc1 suite. No functional changes since 1.0.0-beta1.
- Pin the `drupal/varbase_recipes` to `~1.0.0` dependency for the release.
- Update the version badge to `1.0.0-rc1` in `README.md`.

## [1.0.0-beta1] - 2026-07-09
### Changed
- Update Drupal Core from ~11.3.0 to ~11.4.0 in the Varbase Admin Base recipe.
- Pin the `drupal/varbase_recipes` dependency to `~1.0.0`.
- Update the version badge to `1.0.0-beta1` in `README.md`.
- Run CI on tag pushes and add the README pipeline and release badges.

## [1.0.0-alpha2] - 2026-06-21
### Changed
- Change the logo and emblem to the new approved Varbase brand logo.
- Add the new approved Varbase logo to the `README.md`.

## [1.0.0-alpha1] - 2026-04-26
### Added
- Initial release of the Varbase Admin Base recipe.

[Unreleased]: https://git.drupalcode.org/project/varbase_admin_base/-/compare/1.0.0-rc4...1.0.x
[1.0.0-rc4]: https://git.drupalcode.org/project/varbase_admin_base/-/compare/1.0.0-rc3...1.0.0-rc4
[1.0.0-rc3]: https://git.drupalcode.org/project/varbase_admin_base/-/compare/1.0.0-rc2...1.0.0-rc3
[1.0.0-rc2]: https://git.drupalcode.org/project/varbase_admin_base/-/compare/1.0.0-rc1...1.0.0-rc2
[1.0.0-rc1]: https://git.drupalcode.org/project/varbase_admin_base/-/compare/1.0.0-beta1...1.0.0-rc1
[1.0.0-beta1]: https://git.drupalcode.org/project/varbase_admin_base/-/compare/1.0.0-alpha2...1.0.0-beta1
[1.0.0-alpha2]: https://git.drupalcode.org/project/varbase_admin_base/-/compare/1.0.0-alpha1...1.0.0-alpha2
[1.0.0-alpha1]: https://git.drupalcode.org/project/varbase_admin_base/-/tags/1.0.0-alpha1
