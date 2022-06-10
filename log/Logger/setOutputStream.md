# cge::log::Logger - setOutputStream

`cge::log::Logger::setOutputStream` set the stream where logs will be outputed. It's a [static](https://en.cppreference.com/w/cpp/language/static) methode of [`cge::log::Logger`](./../Logger.md).

## Declaration

```cpp

static void setOutputStream(std::ostream *stream);

```

Parameters:
- `stream` : the [`std::ostream`](https://en.cppreference.com/w/cpp/io/basic_ostream)`*` to output logs. **WARNING :** the stream **MUST** be thread safe or you will have surprise at the output.

## Usage

This static methode is used to set an output stream, that will be used asynchronously, for the log.


# Note

This static methode is declared in the file 'log/log.hpp'.