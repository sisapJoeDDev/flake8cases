# flake8 CASES

### LONG VARIABLES

##### Before
```
self.collector_variables['request_period_in_seconds'] = request_period_in_seconds
```
##### After
```
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
                         "The parameter \"base_tag\" is"
                         "present in the"
                         "config file but the value is"
                         "empty or"
                         "invalid. The base_tag must be"
                         "specified.")
```

### Long array variables

#### Before
```python
indicators_tag =module_definition['module_properties']["indicators_tag"]
```
#### After
```python
lookup_table_name = (
                    module_definition['module_properties']["lookup_table_name"]
                    )
```

### Long variable case

#### Before
```python
days: timedelta = timedelta(self.collector_variables['lookback_days'])
```
#### After
```python
days: timedelta = timedelta(
    self.collector_variables['lookback_days']
    )
```

### Long functions or methods
#### Before
```python
lookup_headers_types.append(self.collector_variables['lookup_header_list'][key])
```
#### After
```python
lookup_headers_types.append(
    self.collector_variables['lookup_header_list'][key])
```

### IF cases

#### Before
```python
if latest_modified_since is None or (event_modified_since > latest_modified_since):
```
#### After
```python
if latest_modified_since is None or\
   (event_modified_since > latest_modified_since):
```
##### continuation line must be indented



