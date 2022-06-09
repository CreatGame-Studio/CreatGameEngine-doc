# cge::log::Log

`cge::log::Log` is a [class](https://en.cppreference.com/w/cpp/language/classes) that handle log data.

## Methodes

- [constructor](./Log/constructor.md)
- [copy](./Log/copy.md)

## Attributes

- [`std::string_view msg`](./Log/msg.md)
- [`std::optional<std::string_view> file`](./Log/file.md)
- [`std::optional<std::string_view> function`](./Log/function.md)
- [`std::optional<int> line`](./Log/line.md)
- [`std::thread::id thread_id`](./Log/thread_id.md)
- [`std::chrono::milliseconds time`](./Log/time.md)
- [`cge::log::Severity severity`](./Log/severity.md)

## Usage

This class is used to store data about a log, like the message, the thread it came from and even sometime the function from where the log was created.
The class is mainly as parameter of [`cge::log::Logger::log`](./Logger/log.md).

## Note

This class is declared in the file 'log/log.hpp'.