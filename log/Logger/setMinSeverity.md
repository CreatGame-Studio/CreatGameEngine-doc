# cge::log::Logger - setMinSeverity

`cge::log::Logger::setMinSeverity` set the minimal log severity to output. It's a [static](https://en.cppreference.com/w/cpp/language/static) methode of [`cge::log::Logger`](./../Logger.md).

## Declaration

```cpp

static void setMinSeverity(cge::log::Severity minSeverity);

```

Parameters:
- `minSeverity` : a [`cge::log::Severity`](./../Severity.md)

## Usage

This static methode is used to set a minimal log severity to output. All logs that have a severity below the given severity won't be outputed.

**Warning**

The given severity **IS** outputed.

# Note

This static methode is declared in the file 'log/log.hpp'.