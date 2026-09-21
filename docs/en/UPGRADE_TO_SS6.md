# Upgrade to Silverstripe 6

This release is a compatibility upgrade for Silverstripe CMS 6. Review the items below before updating your project.

## Requirements

⚠️ BREAKING CHANGE: Upgrade your project to `silverstripe/recipe-core:^6.0` before requiring this version of `sunnysideup/video-embed-extras`.

- Replace any dependency constraints that allow Silverstripe 4 or 5 with Silverstripe 6 equivalents.
- Plan this upgrade as part of a full CMS 6 upgrade. This module no longer declares compatibility with Silverstripe 4 or 5.

## PHP / API compatibility

**🚨 CRITICAL REVIEW REQUIRED / RISKY: Review your PHP runtime before deploying this release. The module now uses the native `#[Override]` attribute in `src/View/ShortCodes/VideoExtras.php`. Confirm that your target PHP version supports it, or verify that your deployment platform tolerates this attribute in your supported runtime.**

- If you maintain forks or project-level overrides of `VideoExtras`, re-test shortcode rendering after the upgrade.
