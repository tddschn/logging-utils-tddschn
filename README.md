## Install
```
$ pip install logging-utils-tddschn
```

## Usage

```python
from logging_utils_tddschn import get_logger

logger, _ = get_logger(__name__)
logger.info('Logging from logging-utils-tddschn!')
```

```
_DEBUG=1 python3 app.py
# prints something like
# INFO:tests.test_utils_naive:/Users/tddschn/app.py:5:<module>:Logging from logging-utils-tddschn!

# logging is turned off (sent to NullHandler) if you don't set env var _DEBUG or it's set to false.
```

