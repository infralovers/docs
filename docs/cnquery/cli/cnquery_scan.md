---
id: cnquery_scan
title: cnquery scan
---

Scan assets with one or more query packs

### Synopsis

This command scans an asset using a query pack. For example, you can scan
the local system with its pre-configured query pack:

    	$ cnquery scan local

To manually configure a query pack, use this:

    	$ cnquery scan local -f bundle.mql.yaml --incognito

```
cnquery scan [flags]
```

### Options

```
      --annotation stringToString     Add an annotation to the asset. (default [])
      --asset-name string             User-override for the asset name
      --detect-cicd                   Try to detect CI/CD environments. If detected, set the asset category to 'cicd'. (default true)
  -h, --help                          help for scan
      --incognito                     Run in incognito mode. Do not report scan results to  Mondoo Platform.
      --inventory-file string         Set the path to the inventory file.
      --inventory-format-ansible      Set the inventory format to Ansible.
      --inventory-format-domainlist   Set the inventory format to domain list.
  -j, --json                          Run the query and return the object in a JSON structure.
  -o, --output string                 Set output format: compact, csv, full, json, json-v1, json-v2, summary, yaml (default "compact")
      --platform-id string            Select a specific target asset by providing its platform ID.
      --props stringToString          Custom values for properties (default [])
      --querypack querypack-bundle    Set the query packs to execute. This requires querypack-bundle. You can specify multiple UIDs.
  -f, --querypack-bundle strings      Path to local query pack file
      --trace-id string               Trace identifier
```

### Options inherited from parent commands

```
      --api-proxy string   Set proxy for communications with Mondoo API
      --auto-update        Enable automatic provider installation and update (default true)
      --config string      Set config file path (default $HOME/.config/mondoo/mondoo.yml)
      --log-level string   Set log level: error, warn, info, debug, trace (default "info")
  -v, --verbose            Enable verbose output
```

### SEE ALSO

- [cnquery](cnquery.md) - cnquery CLI
