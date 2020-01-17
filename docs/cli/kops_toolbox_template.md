
<!--- This file is automatically generated by make gen-cli-docs; changes should be made in the go CLI command code (under cmd/kops) -->

## kops toolbox template

Generate cluster.yaml from template

### Synopsis

Generate cluster.yaml from values input yaml file and apply template.

```
kops toolbox template [flags]
```

### Examples

```
  # generate cluster.yaml from template and input values
  
  kops toolbox template \
  --values values.yaml --values=another.yaml \
  --set var=value --set-string othervar=true \
  --snippets file_or_directory --snippets=another.dir \
  --template file_or_directory --template=directory  \
  --output cluster.yaml
```

### Options

```
      --config-value string      Show the value of a specific configuration value
      --fail-on-missing          Fail on referencing unset variables in templates (default true)
      --format-yaml              Attempt to format the generated yaml content before output
  -h, --help                     help for template
      --output string            Path to output file, otherwise defaults to stdout
      --set stringArray          Set values on the command line (can specify multiple or separate values with commas: key1=val1,key2=val2)
      --set-string stringArray   Set STRING values on the command line (can specify multiple or separate values with commas: key1=val1,key2=val2)
      --snippets strings         Path to directory containing snippets used for templating
      --template strings         Path to template file or directory of templates to render
      --values strings           Path to a configuration file containing values to include in template
```

### Options inherited from parent commands

```
      --alsologtostderr                  log to standard error as well as files
      --config string                    yaml config file (default is $HOME/.kops.yaml)
      --log_backtrace_at traceLocation   when logging hits line file:N, emit a stack trace (default :0)
      --log_dir string                   If non-empty, write log files in this directory
      --log_file string                  If non-empty, use this log file
      --log_file_max_size uint           Defines the maximum size a log file can grow to. Unit is megabytes. If the value is 0, the maximum file size is unlimited. (default 1800)
      --logtostderr                      log to standard error instead of files (default true)
      --name string                      Name of cluster. Overrides KOPS_CLUSTER_NAME environment variable
      --skip_headers                     If true, avoid header prefixes in the log messages
      --skip_log_headers                 If true, avoid headers when opening log files
      --state string                     Location of state storage (kops 'config' file). Overrides KOPS_STATE_STORE environment variable
      --stderrthreshold severity         logs at or above this threshold go to stderr (default 2)
  -v, --v Level                          number for the log level verbosity
      --vmodule moduleSpec               comma-separated list of pattern=N settings for file-filtered logging
```

### SEE ALSO

* [kops toolbox](kops_toolbox.md)	 - Misc infrequently used commands.
