# Changelog

## Version 4.1.0

- Fix [#103](https://github.com/metadevpro/ts-pegjs/pull/103) Fix exception handler export: `PeggySyntaxError` & `DefaultTracer`
- Fix [#104](https://github.com/metadevpro/ts-pegjs/pull/104) Rename grammarSource->source
- Feature [#105](https://github.com/metadevpro/ts-pegjs/pull/105) Add ability to specify `--dependency` style deps by @siefkenj
- Upgrade to `rimraf` 5.0 adding `--glob`

## Version 4.0.0

- [#97](https://github.com/metadevpro/ts-pegjs/pull/97) Ported project to TS. Thansk to @siefkenj
- [#98](https://github.com/metadevpro/ts-pegjs/pull/98) Use os `ts-morph` to infer the type for the rules. Thansk to @siefkenj

## Version 3.2.0

- Added [PR #94](https://github.com/metadevpro/ts-pegjs/pull/93) Converted to vite build and esm. Thansk to @siefkenj

## Version 3.1.0

- Added [PR #91](https://github.com/metadevpro/ts-pegjs/pull/91) Convert new peggy --dependencies or --dependency into TypeScript imports. Thanks to @M00TSDNS

## Version 3.0.0

**Breaking changes!**

- _Breaking change:_ Default for errorName changes from `SyntaxError` to `PeggySyntaxError` from [#86](https://github.com/metadevpro/ts-pegjs/pull/86). Reason: better aligment with Peggy. Allow users to override `SyntaxError` native type.
- _Breaking change:_ Exported Interfaces now does not have the `I` prefix from [#75](https://github.com/metadevpro/ts-pegjs/issues/75). Reason: follow TypeScript conventions for interfaces with no prefix.
  |**Interface**|**Renamed to**|
  |---|---|
  |`IParseOptions`|`ParseOptions`|
  |`ICached`|`Cached`|
  |`ITraceEvent`|`TraceEvent`|
  |`IEndExpectation`|`EndExpectation`|
  |`IOtherExpectation`|`OtherExpectation`|
  |`IAnyExpectation`|`AnyExpectation`|
  |`IClassExpectation`|`ClassExpectation`|
  |`IClassParts`|`ClassParts`|
  |`ILiteralExpectation`|`LiteralExpectation`|
  |`IFileRange`|`FileRange`|
  |`IFilePosition`|`FilePosition`|

## Version 2.2.1

- Fix [#84](https://github.com/metadevpro/ts-pegjs/issues/84) Same convention as peggy. Make `grammarSource` optional.

## Version 2.2.0

- Added support for option `errorName`[#86](https://github.com/metadevpro/ts-pegjs/issues/86) Thanks to @iccicci. Needed after a breaking change in peggy.

## Version 2.1.0

- Add support for the **pluck** operator. Thanks to @hildjj. [#66](https://github.com/metadevpro/ts-pegjs/issues/66)

## Version 2.0.2

- Fix breaking change on peggy-to-plugin integration to receive peggy options. [#79](https://github.com/metadevpro/ts-pegjs/issues/79)

## Version 2.0.1

- Added support for peggy 2.0.1
- Fix [#78](https://github.com/metadevpro/ts-pegjs/issues/78)
- Fix missing helper function

## Version 1.2.2

- Remove prod. dependency for peggy [#65](https://github.com/metadevpro/ts-pegjs/issues/65)
- Added more tests.
- Update libs.

## Version 1.2.1

- Fix src Type for IntelliJ [#70](https://github.com/metadevpro/ts-pegjs/issues/70).

## Version 1.2.0

- Add SyntaxError.format method [#67](https://github.com/metadevpro/ts-pegjs/issues/67).
- Now requires output to be ES6 at minimum (string.repeat needed).

## Version 1.1.1

2021.07.02

- Add missing file to package.json [#64](https://github.com/metadevpro/ts-pegjs/pull/64).

## Version 1.1.0

2021.07.02

- Small changes for peggy [#61](https://github.com/metadevpro/ts-pegjs/pull/61).
- Fixed peggy dependency version [#62](https://github.com/metadevpro/ts-pegjs/pull/62).
- Added top level initializer block [#63](https://github.com/metadevpro/ts-pegjs/pull/63).
- Update libs to latests versions.

## Version 1.0.0

2021.05.26

- Major change: [#59](https://github.com/metadevpro/ts-pegjs/issues/59). Changed dependency from [pegjs](https://github.com/pegjs/pegjs) (unmantained) in favour of [peggy](https://github.com/peggyjs/peggy) (a sensible mantained successor).

## Version 0.3.1

2021.02.09

- Fix [#53](https://github.com/metadevpro/ts-pegjs/issues/53). Errata in `--allowed-start-rules`.

## Version 0.3.0

2020.12.31

- Added ESLint for checking TS.
- Removed support for TSLint rules. Removed options: `noTslint` and `tslintIgnores`
