# Cisco DNA Center CLI

Simple CLI utility to manage DNAC remotely.

Credentials can be set using the following environmental variables

```bash
DNAC_URL 
DNAC_USER 
DNAC_PASSWORD
```

If they are not set, the utility will prompt the user for the information

## Supported subcommands

* add-bulk-pnp-access-point

```bash
% ./dnac_cli add-bulk-pnp-access-point --help
Usage: dnac_cli add-bulk-pnp-access-point [OPTIONS]

  Add APs into DNAC plug and play inventory

Options:
  -i, --inventory-file TEXT      File in CSV format that contains access point
                                 information. Use option -e for an example
                                 [default: ./bulk_pnp_access_point.csv]
  -e, --print-inventory-example  Print example inventory file
  -c, --claim                    Claim devices
  --help                         Show this message and exit.
```

## Install

1. It is strongly recommended to use virtual environments
2. Install dependencies in requirements.txt
3. Test using dnac_cli --help

```bash
% ./dnac_cli --help
Usage: dnac_cli [OPTIONS] COMMAND [ARGS]...

  Top level command

Options:
  --help  Show this message and exit.

Commands:
  add-bulk-pnp-access-point  Add APs into DNAC plug and play inventory
 ```

### Sandbox

If you do not have a DNAC instance available, you can use the [Cisco DNA Center Lab 2](https://devnetsandbox.cisco.com/RM/Diagram/Index/1d94a25e-51bb-48eb-a9c7-dd8eac577953?diagramType=Topology)
to test the script

## Contacts

* Santiago Flores Kanter (sfloresk@cisco.com)