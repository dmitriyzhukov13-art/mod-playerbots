# Random bot equipment progression — proposal for review

This branch shares a focused patch for discussion. It does not modify the module's source files on this branch or apply anything to a running server. The maintainer can review individual changes in `random-bot-gear-progression.patch` and decide whether to adapt or apply them.

The optional progression assigns deterministic equipment item-level ceilings to random bots by level, and applies limits across selection and upgrades. Its default configuration is off.

Important: the current implementation can destroy and regenerate a random bot's equipment on login when it violates a configured cap or character-level requirement. The existing fixed item-level cap can also activate this behavior when optional progression is off. Please review that behavior before considering deployment.

Local Descension verification included a build and selected tests. The patch has been checked for clean application to the fetched upstream files; it has not yet been independently built in a clean upstream environment or benchmarked. OpenAI Codex assisted with implementation and preparation; independent human review is needed.
