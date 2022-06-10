# cge::log::Logger - log

`cge::log::Logger::log` will output a log in the [given stream](./setOutputStream.md). It's a [static](https://en.cppreference.com/w/cpp/language/static) methode of [`cge::log::Logger`](./../Logger.md).

## Declaration

```cpp

static void log(const cge::log::Log &log);

```

Parameters:
- `log` : a `const `[`cge::log::Log`](./../Log.md)`&` that contains all the data of the log to output.

## Usage

This static methode is used to ouput a log in the given output stream. For performance reasons, the log call `cge::log::Logger::_log`, which is a private static methode and handle all ouput process, asynchonously.

**Exemple**

```cpp

cge::log::Logger::log({"A very usefull log", cge::log::Severity::NOTE, __FILE__, __func__, __LINE__});

// output : NOTE [9281] in file '__FILE__', function '__func__', line __LINE__, thread 1 > A very usefull log

```

# Note

This static methode is declared in the file 'log/log.hpp'.