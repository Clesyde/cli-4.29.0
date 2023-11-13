# CLI

Command line interface to facilitate interaction with the Supervisor.

## Usage

- `ha help`
- `ha <subcommand> <action> [<options>]`

E.g.:

- `ha core info --raw-json`

### Modifiers

#### Global

```text
      --api-token string   Supervisor API token
      --config string      Optional config file 
      --endpoint string    Endpoint for Supervisor (default is 'supervisor')
  -h, --help               help for ha
      --log-level string   Log level (defaults to Warn)
      --no-progress        Disable the progress spinner
      --raw-json           Output raw JSON from the API
```

All options are also available as `SUPERVISOR_` prefixed environment variables like `SUPERVISOR_LOG_LEVEL`

#### Subcommands

Available commands:

```text
  addons         Install, update, remove and configure add-ons
  audio          Audio device handling.
  authentication Authentication for users.
  cli            Get information, update or configure the cli backend
  core           Provides control of the Core
  dns            Get information, update or configure the DNS server
  docker         Docker backend specific for info and OCI configuration
  hardware       Provides hardware information about your system
  help           Help about any command
  host           Control the host/system where the core is running on
  info           Provides a general information overview
  multicast      Get information, update or configure the Multicast
  network        Network specific for updating, info and configuration imports
  observer       Get information, update or configure the observer
  os             Operating System specific for updating, info and configuration imports
  resolution     Resolution center of Supervisor, show issues and suggest solutions
  backups        Create, restore and remove backups
  supervisor     Monitor, control and configure the Supervisor
```

## Installation

The CLI is provided by the CLI container on systems and is
available on the device terminal when using the Operating System.

The CLI is automatically updated on those systems.

Furthermore, the SSH add-on (available in the add-on store) provides
access to this tool and several community add-ons provide it as well (e.g.,
the Visual Studio Code add-on).

