# Pull-requests to the upstream KiBoM

This document explains the additions to the original KiBoM code.

## Not yet merged

### Interesting additions

- [Smarter R, L and C sort](Fork_PRs/Smart_sort_for_RLC.md) (#82)
- [Links to datasheet in a configurable column](Fork_PRs/Datasheet_as_link.md) (#112)

### Small additions

- [Optimize the regex used to match component values](Fork_PRs/Optimize_units_regex.md) (#110)

### Small fixes

- [Fix extra parameter in getAltRefs](Fork_PRs/Fix_getAltRefs) (#119)

## Already merged

### Interesting additions

- [Mark components as "Do Not Change" (DNC)](Fork_PRs/DNC.md)
- [Separate section for "Do Not Fit" components](Fork_PRs/Separate_DNF.md)
- [Join fields to make the BoM more compact](Fork_PRs/Join_fields.md)
- [Links to Digi-Key in a configurable column](Fork_PRs/Link_to_digikey.md)
- [Command line compatibility with older versions](Fork_PRs/CLI_compatibility.md)

### Small additions

- [Support space as separator in the Config field](Fork_PRs/Space_in_config.md)
- [Use "M" for "mega" and "m" for "milli"](Fork_PRs/Mega_prefix.md)
- [Avoid destroying the current locale's decimal point](Fork_PRs/Use_locale_decimal_point.md)
- [Add support for spaces between a value an its unit](Fork_PRs/Space_before_unit.md)

### Small fixes

- [Component description fallback for KiCad 5.x](Fork_PRs/Description_Fallback.md)
- [Avoid exposing the local path in the output name](Fork_PRs/No_path_in_name.md)
- [Avoid data files marked as executables](Fork_PRs/No_executable_data.md)
- [+VARIANT mechanism not working as expected](Fork_PRs/Variant_plus.md)
- [Skip the DNF HTML list if it will contain 0 rows](Fork_PRs/Skip_empty_DNF_table.md)


## Not sent to upstream

- Debian package files. Allowing to install KiBoM as a Debian package on Debian, Ubuntu and derevatives. Making it clean and simple to install, uninstall and get its dependencies.
- Integration with GitHub actions, instead of using Travis.
- PyTest regression tests.
  - Stronger test for generated CSV
  - Basic test for generated HTML
  - Basic test for generated XML
  - Basic test for generated XLSX
  - Basic test for variants
  - Basic test for DNC
  - Test for component sorting (by value)
