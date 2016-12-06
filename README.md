# chianer_log_report_csv

`LogReport` extension in [chainer](https://github.com/pfnet/chainer)  which supports csv output

## Requirements

- [pandas](http://pandas.pydata.org/)

  If you use [Anaconda](https://www.continuum.io/downloads) environment, pandas has been already installed.

## Usage

```python
from log_report import LogReport


# in trainer setup phase,
trainer.extend(LogReport(trigger=log_interval, type='csv'))
```

In default, `type='json'` is specified, and in this case, it is completely same as [original `LogReport` implementation](http://docs.chainer.org/en/stable/reference/extensions.html#logreport)

