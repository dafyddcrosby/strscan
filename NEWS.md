# News

## 3.0.1 - 2021-10-23

### Fixes

  * Fixed a segmentation of `StringScanner#charpos` when
    `String#byteslice` returns non string value.
    [Bug #17756][GitHub#20][Patch by Kenichi Kamiya]

### Thanks

  * Kenichi Kamiya

## 1.0.3 - 2019-10-14

### Improvements

  * Stopped depending on `regint.h`.

### Fixes

  * Fixed a bug that a build flag is ignored when this is installed by
    `gem install`.
    [GitHub#7][Reported by Michael Camilleri]

### Thanks

  * Michael Camilleri

## 1.0.2 - 2019-10-13

### Improvements

  * Added support for `String` as a pattern. This improves performance.
    [GitHub#4]

  * Improved documentation.
    [GitHub#8][Patch by Espartaco Palma]

  * Added tests for anchors.
    [GitHub#9][Patch by Jeanine Adkisson]

  * Added support for fixed anchor mode. In this mode, `\A` matches to
    the beginning of source string instead of the current
    position. `^` matches to the begging of line instead of the
    current position.

    You can use fixed anchor mode by passing `fixed_anchor: true`
    option to `StringScanner.new` such as `StringScanner.new(string,
    fixed_anchor: true)`.

    `StringScanner#fixed_anchor?` is also added to get whether fixed
    anchor mode is used or not.

    [GitHub#6][Patch by Michael Camilleri]
    [GitHub#10]

### Thanks

  * Espartaco Palma

  * Michael Camilleri

  * Jeanine Adkisson
