# Python.

For manage python installation:
```yaml
python_version:     "3.11.4"
python_source_path: "/usr/local/python"
```

## Build.
Build and install python from source on local machine.  
_(it's take a time)_
  
For manage configuration:
```yaml
python_build_options: [
  "--enable-optimizations",
  "--enable-optimizations",
  "--without-tests",
  "--without-tk",
]
```

### Supported Platforms:
- Debian-based Linux distributions
- RedHat-based Linux distributions
