# FoxVale Seekers Privacy Policy

Effective October 24, 2026.

FoxVale Seekers is operated by the FoxVale community through u/FoxValeSMP. It helps FoxVale staff discover public requests from adults who may want to join its Minecraft survival community. It reads requests, identifies possible matches, and sends private Discord alerts for human review. It does not contact people or make membership decisions.

## Information processed

The app reads post titles, bodies, public post links and IDs, creation times, community names, request flair, crosspost references, and removal or reply restrictions in these communities: MinecraftBuddies, MinecraftServer, MinecraftServerFinder, MinecraftSMPs, MinecraftServers, smp, and MCVanillaServers. It compares the request with FoxVale's gameplay and community requirements using fixed rules. Missing details remain uncertain.

It does not inspect player profiles or posting histories, link Reddit identities to Discord accounts, infer sensitive characteristics, sell data, train AI models, or send requests to an AI service. Posts may contain information their authors chose to include; staff must use it only to review that server request.

## Storage and recipients

Reddit Devvit hosts the app. Raw requests are processed transiently. Devvit Redis stores feed checkpoints, post IDs, hashes for duplicate and change detection, and Discord delivery IDs. It does not intentionally store author names or account IDs. Operational logs contain counts, timestamps, community names, delivery IDs, and failure status rather than request bodies or secrets.

Alerts sent to Discord include a title, request excerpt, Reddit link, possible gameplay fit, and relevant uncertainties. Only the designated FoxVale staff channel receives these alerts. Discord processes those messages under its own [privacy policy](https://discord.com/privacy). The webhook credential is stored in Devvit's encrypted secret setting. GitHub hosts these public policy documents; no player requests or credentials are published in this repository.

## Retention and changes to source posts

The production configuration checks approximately every five minutes. It rechecks tracked source posts and removes its webhook alert if it detects deletion, moderator removal, or a change to the stored request content. Alerts also expire after seven days. The app retains tracking metadata until Discord confirms deletion so a failed deletion can be retried. API outages or backlogs can delay checks and deletion; new alerts stop when cleanup fails or falls behind. Staff must investigate those failures promptly.

Duplicate markers normally expire after 30 days, content duplicate hashes after seven days. Delivery cleanup replaces source metadata with a minimal deletion/deduplication marker. Checkpoints retain one timestamp per community while the app operates. Disabling new alerts leaves scheduled cleanup enabled. Before uninstalling or stopping the app permanently, the operator must remove remaining app-created Discord copies and clear the app's stored data.

Staff must not copy alert excerpts into other systems or use them to build player dossiers. Existing messages sent by the earlier Holly browser-monitor prototype are outside the new webhook's automatic cleanup and require operator removal when applicable. This policy does not promise deletion of copies independently made by Discord users or retention controlled by platform providers.

## Questions and deletion requests

Contact [u/FoxValeSMP](https://www.reddit.com/user/FoxValeSMP/) on Reddit about this app, a correction, or deletion. Include the Reddit post link or ID; do not send a password, identity document, or other unnecessary personal information. The operator can remove and suppress a post's alert without inspecting its author's history. Requests are handled manually, and changes are applied to the app's copies. The original Reddit post remains controlled by its author and Reddit.

This policy applies to FoxVale Seekers. It does not replace Reddit's, Discord's, or GitHub's own policies. The app is not affiliated with or endorsed by Reddit, Discord, Microsoft, or Mojang.
