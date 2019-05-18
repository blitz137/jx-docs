---
date: 2019-05-18T14:59:07Z
title: "jx get cve"
slug: jx_get_cve
url: /commands/jx_get_cve/
---
## jx get cve

Display Common Vulnerabilities and Exposures (CVEs)

### Synopsis

Display Common Vulnerabilities and Exposures (CVEs)

```
jx get cve [flags]
```

### Examples

```
  # List all Common Vulnerabilities and Exposures (CVEs)
  
  jx get cve # using current dir as the context for app name
  jx get cve --app foo
  jx get cve --app foo --version 1.0.0
  jx get cve --app foo --environment staging
  jx get cve --environment staging
```

### Options

```
  -e, --environment string   The Environment to find running applications
  -h, --help                 help for cve
      --image-id string      Image ID in CVE engine if already known
      --image-name string    Full image name e.g. jenkinsxio/nexus 
      --version string       Version or tag e.g. 0.0.1
```

### Options inherited from parent commands

```
  -b, --batch-mode                Runs in batch mode without prompting for user input (default true)
      --install-dependencies      Enables automatic dependencies installation when required
      --log-level string          Sets the logging level (panic, fatal, error, warning, info, debug) (default "info")
      --no-brew                   Disables brew package manager on MacOS when installing binary dependencies
      --skip-auth-secrets-merge   Skips merging the secrets from local files with the secrets from Kubernetes cluster
      --verbose                   Enables verbose output
```

### SEE ALSO

* [jx get](/commands/jx_get/)	 - Display one or more resources

###### Auto generated by spf13/cobra on 18-May-2019