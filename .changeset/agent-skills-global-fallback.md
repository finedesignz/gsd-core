---
type: Fixed
pr: 1
---
**`agent_skills` in `~/.gsd/defaults.json` now applies inside projects** - a project config that does not define an agent key inherits the global skills for that agent, a project value overrides it, and an explicit empty array still opts out. Previously the global value was ignored whenever `.planning/config.json` existed, and only warned about it.
