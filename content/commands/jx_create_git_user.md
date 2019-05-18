---
date: 2019-05-18T14:59:07Z
title: "jx create git user"
slug: jx_create_git_user
url: /commands/jx_create_git_user/
---
## jx create git user

Adds a new user to the Git server

### Synopsis

Creates a new user for a Git Server. Only supported for Gitea so far

```
jx create git user [username] [flags]
```

### Examples

```
  # Creates a new user in the local Gitea server
  jx create git user -n local someUserName -p somepassword -e foo@bar.com
```

### Options

```
  -a, --admin              Whether the user is an admin user
  -t, --api-token string   The API Token for the user
  -e, --email string       The User email address
  -h, --help               help for user
  -n, --name string        The name of the Git server to add a user
  -p, --password string    The User password to try automatically create a new API Token
  -u, --url string         The URL of the Git server to add a user
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

* [jx create git](/commands/jx_create_git/)	 - Creates a Git resource

###### Auto generated by spf13/cobra on 18-May-2019