<img src="https://phpmath.github.io/assets/favicon.svg" width="72" height="72" alt="phpmath">

# phpmath

**Precise math for modern PHP.** Immutable, fully tested libraries that follow one standard, so they all work the same way.

Website and documentation: **https://phpmath.github.io**

## Libraries

| Library | What it does |
|---|---|
| [biginteger](https://github.com/phpmath/biginteger) | Integers of any size, built on GMP. |
| [bignumber](https://github.com/phpmath/bignumber) | Decimal numbers of any size and precision, built on bcmath. |
| [fraction](https://github.com/phpmath/fraction) | Exact rational numbers that never lose precision. |
| [vector](https://github.com/phpmath/vector) | Vectors in two, three, four and more dimensions. |
| [matrix](https://github.com/phpmath/matrix) | Matrices with determinants, inverses and 3D transformations. |
| [complex](https://github.com/phpmath/complex) | Complex numbers with polar form, powers and roots. |
| [quaternion](https://github.com/phpmath/quaternion) | Quaternions for 3D rotation, with axis-angle and slerp. |
| [polynomial](https://github.com/phpmath/polynomial) | Polynomials with arithmetic, calculus and real roots. |
| [number-theory](https://github.com/phpmath/number-theory) | Primes, factorization and modular arithmetic. |
| [statistics](https://github.com/phpmath/statistics) | Descriptive statistics, the normal distribution and regression. |
| [geometry](https://github.com/phpmath/geometry) | Points, lines, circles, rectangles and polygons. |

Tooling: [coding-standard](https://github.com/phpmath/coding-standard) is the shared PHP_CodeSniffer standard and [docs-builder](https://github.com/phpmath/docs-builder) builds the documentation sites.

## Principles

- **Immutable.** Every number, vector and matrix is a value object that never changes.
- **Consistent.** The same coding standard, structure, exceptions and documentation everywhere.
- **Modern PHP.** Only actively supported PHP versions, strict types and native types.
- **Well tested.** 100% coverage and PHPStan at the maximum level on every change.

Every library installs with Composer, for example `composer require phpmath/matrix`.
