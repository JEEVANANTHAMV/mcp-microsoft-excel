# Microsoft Excel

> Automates Microsoft Excel through this assistant — build and edit workbooks, tables, pivot tables, charts, and formulas. Needs Microsoft Excel 2016 or newer installed.

The bundle zip (**62.6 MB**) is stored in this repository at **`ffabeede-c64b-430e-b642-d1408e0c782b.zip`**.

This repository is part of the **Forjinn-Desk** MCP bundle collection. An MCP bundle is a self-contained server that a host application launches and communicates with over the MCP (Model Context Protocol) protocol.

## Repo metadata

| Field | Value |
| --- | --- |
| Registry ID | `ffabeede-c64b-430e-b642-d1408e0c782b` |
| Status in registry | active |
| Bundle size | 62.6 MB |
| Distribution | committed to this repo |

## Environment variables

| Variable | Value / note |
| --- | --- |
| `EXCEL_INSTALL_PATH` | `C:\Program Files\Microsoft Office\root\Office16\EXCEL.EXE` |

## MCP launch configuration

The host replaces `__INSTALL_DIR__` (install dir) and `__PYTHON__` (bundled Python) at runtime.

```json
{
  "command": "__INSTALL_DIR__\\mcp-excel.exe",
  "args": [],
  "env": {
    "EXCEL_INSTALL_PATH": "C:\\Program Files\\Microsoft Office\\root\\Office16\\EXCEL.EXE"
  }
}
```


## Install / usage

1. Get the bundle:
   - download `ffabeede-c64b-430e-b642-d1408e0c782b.zip` from this repo (Code → Download ZIP, or `git clone`).
2. Extract to your target installation directory (config paths expect contents at the install-dir root).
3. Set the environment variables listed above.
4. Launch using the MCP config JSON (or let a host client manage it automatically).

> Bundles may include vendored runtimes (bundled Python, Node, or native executables). Builds are Windows x64.
