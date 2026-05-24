# Why local-first wellness agents need MCP

AI agents are most useful when they understand the real constraints of the person they serve. For health, training and recovery work, that context is not abstract. It is sleep, HRV, strain, nutrition, glucose, cycle phase, air quality, schedule, preferences and the user's own boundaries.

Most of that data is sensitive. A useful agent stack should not require a hosted token vault, a private data copy or a new dashboard between the user and their existing tools. The default should be local-first: credentials stay on the user's machine, tools expose structured summaries, and raw data is opt-in.

That is the operating thesis behind Delx Wellness.

## The problem

Wearables and nutrition apps already produce high-signal data, but they are fragmented:

- WHOOP knows recovery, HRV, strain and sleep.
- Garmin knows Body Battery, training readiness, stress and activities.
- Oura, Fitbit, Strava, Withings, Apple Health, Samsung Health and Polar all expose different slices of the same human operating picture.
- Nutrition data lives across food search, barcode lookup, photos, hydration and local meal memory.

Agents cannot act well if every connector has a different auth story, response shape, privacy boundary and readiness check.

## The approach

Delx Wellness turns these sources into installable MCP servers and profile packs:

- `delx-wellness` is the public registry and source of truth.
- `wellness-nourish` is the local nutrition layer.
- `whoop-mcp`, `garminmcp`, `strava-mcp` and the other connectors expose provider-specific signals.
- `delx-wellness-hermes` and `delx-wellness-openclaw` install the stack as one local profile.
- `delx-agent-workbench` gives builders runnable examples, prompts and MCP client configs.

The goal is not to make a medical oracle. The goal is to make personal context available to the agent in a controlled, inspectable and reversible way.

## The standard

Every serious connector should make these surfaces obvious:

- A one-command install or setup path.
- A `connection_status` or doctor-style readiness check.
- A privacy model that explains where credentials and data live.
- A small set of high-value summary tools before raw payload access.
- A safe default for mutations, uploads and irreversible actions.
- A README that shows an agent what to call first.

## Start here

- Registry: https://github.com/davidmosiah/delx-wellness
- Nutrition: https://github.com/davidmosiah/wellness-nourish
- WHOOP: https://github.com/davidmosiah/whoop-mcp
- Garmin: https://github.com/davidmosiah/garminmcp
- Hermes profile: https://github.com/davidmosiah/delx-wellness-hermes
- Workbench: https://github.com/davidmosiah/delx-agent-workbench

If this direction is useful, star the registry first. Stars help other builders find the map; npm downloads tell me which connectors are actually getting installed.
