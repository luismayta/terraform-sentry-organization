### sentry organization

```hcl

  module "sentry" {
    providers = {
      sentry = sentry
    }
    source      = "hadenlabs/organization/sentry"
    version     = "0.1.0"
    name        = "name organization"
  }

```

### sentry organization with teams

```hcl

  module "sentry" {
    providers = {
      sentry = sentry
    }
    source      = "hadenlabs/organization/sentry"
    version     = "0.1.0"
    name        = "name organization"
    teams       = [
      {
        name = "team 1"
      }
    ]

  }

```
