#v2.0.0
- Breaking: Upgraded ember-cli and ember to 1.13 series, tests no longer pass against ember 1.11 and so compatibility is now >=1.12.0. 
  Suspect the addon will still work under 1.11 and that the failures are due to ember-cli interactions.
- Eliminate deprecations in app and test suite

#v1.1.0
- Upgrade ember-cli

#v1.0.0
- 1.0 because its been used in production for months and we're making changes with nice deprecations
- `resetFeatureFlags` is no longer necessary to reset flags between tests; flags are not shared between app instances anymore
- `enabled` renamed to `isEnabled`
- Flags should now be set via the `featureFlags` key in the config, rather than `APP.FEATURES`
- The service name can now be customized using `featureFlagsService` config 

#v0.0.4
- Upgrade to ember-cli 0.0.2

#v0.0.3
- Breaking change: Remove use of window.Features; flags can now be specified in config or explicitly setup with `features.setup`
- Breaking change: Remove handlebars helper - compatibility with htmlbars
- Feature: Feature flags are now bound in templates with regular `if` statements, in a camelized form ('new-feature' becomes 'newFeature'). See Readme.
- Bugfix: Logging now turns off if the config flag is off.

#v0.0.1, v0.0.2
- Initial commit
