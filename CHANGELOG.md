master (unreleased)
* Teach scss-lint to prefer hexadecimal colors over color names

0.9.0
* Add `--show-linters` flag for listing all linters available to scss-lint
* Change `--ignore-linter` flag to use `CamelCase` linter names instead of
  `snake_case`
* Removed `-x` alias for `--xml` flag
* Change `-i`/`--ignore-linter` flags to `-x`/`--exclude-linter`
* Add `-i`/`--include-linters` flag to specify a subset of linters
* Fix bug where using transform-related functions were reported as lints
* Teach scss-lint that `.5em` is preferred over `0.5em`
* Teach scss-lint to prefer lowercase characters in selectors
* Linters names no longer have a `Linter` suffix
* Teach scss-lint that `@extend` should use placeholder selectors
* Fix bug where a lint would be reported for hyphened keyword arguments
* Teach scss-lint to recognize vendor-prefixed properties when enforcing sort
  order

0.8.0
* Handle non-existent files/directories gracefully
* Teach scss-lint that opening curly braces should be preceded by one space
* Teach scss-lint that placeholder names should be lowercase and use hyphens

0.7.1
* Upgrade Sass gem dependency from 3.2.8 -> 3.2.9
* Fixed crash that occurred for directive nodes (`@media`, etc.)

0.7.0
* Teach scss-lint that `border: 0;` is preferred over `border: none;`
* Teach scss-lint that variable names should not contain underscores or capital
  letters
* Teach scss-lint that function and mixin names follow same rules as variables
* Fix shorthand linter to work with Sass script expressions
* Fix property format linter to work with interpolated expressions
* Teach scss-lint to check names of functions/mixins/variables in scripts
* Fix hex color linter to work with Sass script expressions
* Teach scss-lint that // comments should be preferred over /**/ comments
* Upgrade Sass gem dependency from 3.2.7 -> 3.2.8

0.6.7
* Fixed `--ignore-linters` flag

0.6.6

* Fixed `--version` flag to not error due to not autoloading `VERSION`
* Trailing newlines are no longer output by default in linter output

0.6.5

* Major refactor of the Linter class to use Visitor pattern
* Fix shorthand linter for lists containing function calls

0.6

* Only lint files with `css` or `scss` extensions
* Fix recursive directory scanning
* Fix specs on Sass gem >= 3.2.6 (shorthand_linter was failing)
* Add changelog (the thing you're reading)
* Add command-line flags (e.g. --version, --help)
* Add --xml flag for outputting XML
* Add --exclude flag for excluding SCSS files from being linted
* Add --ignore-linters flag to skip lints produced by certain linters

0.5.2

* Version bump to remove erroneously added untracked files from gem

0.5

* Improve clarity of shorthand linter through naming
* Teach scss-lint `property: 10px 10px` can be shorter
* Clarify ShorthandLinter spec structure

0.4

* Add linter for unnecessary types in selectors

0.3

* Teach scss-lint that selectors each get their own line

0.2

* Teach scss-lint about nested property syntax
* Teach scss-lint to detect too-long shorthand values
* Make scss-lint detect space before semicolon
* Add linter for order of declarations

0.1

* Initial public release
