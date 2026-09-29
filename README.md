# com.kruty1918.connectivity

Reusable connectivity monitoring: internet reachability probes, online/offline
status events, and wait-for-connectivity helpers.

## Install (Unity Package Manager)

Package Manager → **+** → **Add package from git URL**:

```
https://github.com/kruty1918dev-ai/com.kruty1918.connectivity.git
```

or in `Packages/manifest.json`:

```json
"com.kruty1918.connectivity": "https://github.com/kruty1918dev-ai/com.kruty1918.connectivity.git#v0.1.0"
```

The repository is private — Git credentials (PAT / Git Credential Manager)
are required on every machine that resolves the package.

## API surface

| Type | Purpose |
|---|---|
| `IConnectivityService` | Reachability probes, online/offline status events, `await`-able wait-for-connectivity helpers |

## Model

Reusable UPM package extracted from Moyva. No game-specific dependencies;
compose via your own installer/DI. Useful for gating online features
(lobby/relay flows, telemetry upload) on real connectivity rather than
`Application.internetReachability` alone.
