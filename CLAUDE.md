# qqq-app-developer-intellij-plugin

IntelliJ plugin ("QQQ App Developer Tools", Marketplace plugin 24725) providing
file templates and live templates for QQQ application development. Pure-resource
plugin — no Java/Kotlin code; all content lives under `src/main/resources/`
(`fileTemplates/`, `liveTemplates/`, `META-INF/plugin.xml`).

Build: `./gradlew buildPlugin` | dev loop: `./gradlew runIde` | publish (manual):
`signPlugin` + `publishPlugin` with env vars (see `build.gradle.kts`).

## Knowledge base

- Platform hub: `R:/Git.Local/KofTwentyTwo/second-brain/knowledge/qqq/qqq-hub.md`
- This repo's dossier: `R:/Git.Local/KofTwentyTwo/second-brain/knowledge/qqq/repos/qqq-app-developer-intellij-plugin.md`
- Reviewed commit: `dd76c1b11519` (branch `main`, 2026-07-04 deep review)

Key facts from the review: zero qqq artifact dependencies (coupling is textual —
templates emit `com.kingsrook.qqq.backend.core.*` code); Marketplace version
1.1.0 unchanged since 2024-07-12; LICENSE is AGPL-3.0 (QRun-IO copyright, added
2025-12-25); template-emitted APIs verified to survive the v4.0 BREAK-03/04
removals.
