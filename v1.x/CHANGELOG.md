
# Change Log

All notable changes to this project will be documented in this file.
This project adheres to [Semantic Versioning](http://semver.org/).

## [1.6.3](https://github.com/VDS13/telegram-inline-calendar/compare/1.6.2...1.6.3) - 2023-07-18

### Added:

* Turkish language support.

## [1.6.2](https://github.com/VDS13/telegram-inline-calendar/compare/1.6.1...1.6.2) - 2023-03-16

### Added:

* ESM Support Information.

## [1.6.1](https://github.com/VDS13/telegram-inline-calendar/compare/1.6.0...1.6.1) - 2023-03-05

### Changed:

* Fix examples.

## [1.6.0](https://github.com/VDS13/telegram-inline-calendar/compare/1.5.0...1.6.0) - 2023-03-03

### Added:

* Option `custom_start_msg` to change the text of the message sent with the calendar/time selector.

Example:
```js
const calendar = new Calendar(bot, {
    date_format: 'DD-MM-YYYY',
    language: 'en',
    bot_api: 'grammy',
    custom_start_msg: 'Сustom start message'
});
```
<div align="left">
<img src="https://github.com/VDS13/telegram-inline-calendar/blob/main/img/ex3.jpg" width="200"/>
</div>

## [1.5.0](https://github.com/VDS13/telegram-inline-calendar/compare/1.4.0...1.5.0) - 2023-02-22

### Added:

* Options `start_date` and `stop_date` to limit the pool of dates in the calendar.

Example:
```js
const calendar = new Calendar(bot, {
    date_format: 'DD-MM-YYYY',
    language: 'en',
    bot_api: 'grammy',
    start_date: '2022-11-15',
    stop_date: '2023-04-20'
});
```
<div align="left">
<img src="https://github.com/VDS13/telegram-inline-calendar/blob/main/img/ex1.jpg" width="200"/>
<img src="https://github.com/VDS13/telegram-inline-calendar/blob/main/img/ex2.jpg" width="200"/>
</div>

Note: 
```js
start_date <= new Date() <= stop_date
```

## [1.4.0](https://github.com/VDS13/telegram-inline-calendar/compare/1.3.3...1.4.0) - 2023-01-25

### Added:

* Support for [`grammy`](https://github.com/grammyjs/grammY) library

### Changed:

* Library optimization.
* Fixed bugs in `EXAMPLES.md` and `README.md`

## [1.3.3](https://github.com/VDS13/telegram-inline-calendar/compare/1.3.2...1.3.3) - 2023-01-22

### Changed:

* Library optimization.

## [1.3.2](https://github.com/VDS13/telegram-inline-calendar/compare/1.3.1...1.3.2) - 2023-01-14

### Changed:

* Hotfix ```README.md```.

## [1.3.1](https://github.com/VDS13/telegram-inline-calendar/compare/1.3.0...1.3.1) - 2023-01-14

### Changed:

* Hotfix ```README.md```.

## [1.3.0](https://github.com/VDS13/telegram-inline-calendar/compare/1.2.1...1.3.0) - 2023-01-14

### Added:

* Time selector (can be used in conjunction with the calendar and separately).
More details in the [API](https://github.com/VDS13/telegram-inline-calendar/blob/main/API.md) and [examples](https://github.com/VDS13/telegram-inline-calendar/blob/main/EXAMPLES.md)

## [1.2.1](https://github.com/VDS13/telegram-inline-calendar/compare/1.2.0...1.2.1) - 2023-01-14

### Changed:

* Hotfix ```close_calendar```.

## [1.2.0](https://github.com/VDS13/telegram-inline-calendar/compare/1.1.2...1.2.0) - 2023-01-12

### Added: ([issues#2](https://github.com/VDS13/telegram-inline-calendar/issues/2))

* Option `start_week_day`, which sets the first day of the week (Sunday - `0`, Monday - `1`, Tuesday - `2` and so on).

## [1.1.2](https://github.com/VDS13/telegram-inline-calendar/compare/1.1.1...1.1.2) - 2023-01-02

### Changed: ([issues#1](https://github.com/VDS13/telegram-inline-calendar/issues/1))

* Fixed bug with `callback_data` overflow.

## [1.1.1](https://github.com/VDS13/telegram-inline-calendar/compare/1.1.0...1.1.1) - 2022-12-22

### Changed:

* Hotfix ```close_calendar```.

## [1.1.0](https://github.com/VDS13/telegram-inline-calendar/compare/1.0.3...1.1.0) - 2022-12-22

### Added:

* Option ```close_calendar```, which determines whether to close the calendar after selecting a date.