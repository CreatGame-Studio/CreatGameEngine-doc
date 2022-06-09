# cge::log::Log - constructor

## Declaration

```cpp

/* 1 */ Log() = default;
/* 2 */ Log(std::string_view _msg, cge::log::Severity _severity, std::optional<std::string_view> _file, std::optional<std::string_view> _function, std::optional<int> _line);

```

2. Parameters :
	- `_msg` : A [`string_view`](https://en.cppreference.com/w/cpp/string/basic_string_view) that contain the message of the log
	- `_severity` : An [`cge::log::Severity`](./../severity.md) enum that indicates the severity of the log.
	- `_file` : An [optional](https://en.cppreference.com/w/cpp/utility/optional) [`std::string_view`](https://en.cppreference.com/w/cpp/string/basic_string_view) that can contain the name of the file where the log was created. Default to not initialized => `_file.has_value() = false`;
	- `_function` : An [optional](https://en.cppreference.com/w/cpp/utility/optional) [`std::string_view`](https://en.cppreference.com/w/cpp/string/basic_string_view) that can contain the name of the function where the log was created. Default to not initialized => `_function.has_value() = false`;
	- `_function` : An [optional](https://en.cppreference.com/w/cpp/utility/optional) `int` that can contain the line where the log was created. Default to not initialized => `_line_.has_value() = false`;

## Usage

You can use all those constructors just with `{...}` as parameter of [`cge::log::Logger::log`](./../Logger/log.md).

**Warning**

If you use the second constructor like this for exemple : `{"A very usefull message", cge::log::Severity::ERROR, "main.cpp"}`, the `file` attribute of [`cge::log::Log`](./../Log.md) will just be useless if you don't initialize `function` and `line`.

## Note

Those methodes are declared in the file 'log/log.hpp'.