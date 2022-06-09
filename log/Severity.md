# cge::log::Severity

`cge::log::Severity` is an enumration that represent different level of log severity.

## Declaration

```cpp

namespace cge::log
{
	enum class Severity
	{
		DEBUG = 0,
		NOTE,
		PERFORMANCE,
		WARNING,
		ERROR
	};
}

```

## Usage

This enumration is used only be `cge::log::Log`. It contains the severity of the log printed. It's made so you can select easly a minimal severity like this :

```cpp

cge::log::Severity severity {/* severity of the log */};
cge::log::Severity minAcceptedSeverity {/* the lowest log you want to take care of */};

if (severity >= minAcceptedSeverity)
{
	// the log is sufficiently serious to take care of it
}


```

## Note

This enumration is declared in the file 'log/log.hpp'.