# mountOS
A cross-platform, forkable, time-traveling distributed filesystem over object storage.

Mount it natively on macOS, Windows, Linux, and Kubernetes, or reach it over S3 and WebHDFS, on owned infrastructure. A single deployment is free up to 10 TiB.

## Start here

- [Get started](https://mountos.io/docs/get-started)
- [Use cases](https://mountos.io/use-cases)
- [Documentation](https://mountos.io/docs)
- [Product overview](https://mountos.io/product)

## Repositories

| Repository | Purpose |
| --- | --- |
| [skills](https://github.com/mountos-io/skills) | Agent skills to deploy, integrate, operate, and troubleshoot mountOS |
| [mountos-admin-sdk](https://github.com/mountos-io/mountos-admin-sdk) | TypeScript, Go, and Rust SDKs |
| [mountos-desktop](https://github.com/mountos-io/mountos-desktop) | Desktop app for macOS and Windows |
| [mountos-admin-client](https://github.com/mountos-io/mountos-admin-client) | Open-source admin dashboard |
| [mountos-hdfs-sdk](https://github.com/mountos-io/mountos-hdfs-sdk) | Hadoop filesystem jar for Spark, Hive, Trino, and Flink |
| [deployment](https://github.com/mountos-io/deployment) | Terraform for AWS, Azure, and GCP |


## For AI agents

- [Agent skills](https://github.com/mountos-io/skills): drop-in skills to deploy, integrate, operate, and troubleshoot mountOS
- [Skill index](https://mountos.io/skill.md): one file that lists every skill
- [llms.txt](https://mountos.io/llms.txt): documentation index for language models
- [Full corpus](https://mountos.io/ai/llms-full.txt): all topics in one file
- [Agent guide](https://mountos.io/ai/AGENTS.md): how an agent should work with mountOS
- [Use with AI agents](https://mountos.io/docs/ai): setup for coding assistants

Product, use-case, and documentation pages return Markdown when a client sends `Accept: text/markdown`.

## Install

macOS and Linux:

```sh
curl -fsSL https://mountos.sh/install | bash
```

Windows (PowerShell):

```powershell
Invoke-WebRequest https://mountos.sh/install/install.ps1 -OutFile mountos.ps1; .\mountos.ps1
```

On macOS and Windows the installer adds the full client bundle (desktop app and `mountos` CLI). On Linux it installs the `mountos` CLI. It detects platform and architecture and verifies the SHA-256 checksum before it extracts.

Install a specific version, or only the CLI:

```sh
curl -fsSL https://mountos.sh/install | bash -s -- --pkg mountos-cli --version 1.2.3
```

Add `--list` to see available versions. Server services ship as e `--pkg mountos-dataserv`. Full options:[mountos.io/docs/download](https://mountos.io/docs/download).

Contact: [mountos.io/contact](https://mountos.io/contact) or support@mountos.io
