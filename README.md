# flake8 CASES

### Long variables

##### Before
```python
self.collector_variables['request_period_in_seconds'] = request_period_in_seconds
```
##### After
```python
self.collector_variables[
                         'request_period_in_seconds'
                        ] = request_period_in_seconds
```

### Long strings

##### Before
```python
raise InitVariablesError(10,
                         "The parameter \"base_tag\" is present in the"
                         "config file but the value is empty or"
                         "invalid. The base_tag must be specified.")
```
##### After
```python
raise InitVariablesError(10,
						 "The parameter \"base_tag\" is present in the"
                         "config file but the value is empty or"
                         "invalid. The base_tag must be specified.")
```

