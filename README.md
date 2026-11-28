# CA Policy Analyzer

[日本語版 README](README_ja.md)

**Do admin exclusions or legacy authentication gaps remain in your Conditional Access policies?**

## What is this tool?

CA Policy Analyzer is a Windows desktop app by Sumikko Lab, built as a tool to analyze Conditional Access policies. It loads policy JSON and analyzes it on your PC without connecting to your tenant. The app connects to Microsoft Store for license checks and purchases.

## What it does

- Gap analysis: compares your policies with 28 recommended items (Microsoft 16, DISA STIG 5, NIST SP 800-53 7).
- Admin exclusion analysis: shows the recommended items where admin groups are excluded, and whether admin-only policies cover them.
- Coverage analysis: shows gaps that remain across your policies, and groups excluded from many all-user policies.
- Change history: records the name and reason you enter when you load JSON, and shows the differences.
- Simulation (Pro): checks whether a sign-in is blocked for the users, apps and other conditions you specify.
- Excel design document (8 sheets) and PDF report export (Pro), with automated diagnostics such as conflicts, duplicates, and policies that block all users and all apps with no exclusions. To include diagnostics, run Compare with Recommended Config before you export.

## Out of scope

- Policies are loaded from files or registered on screen (retrieving them from your tenant and changing tenant settings are out of scope).
- The app loads policy JSON in its own format. Convert Entra admin center or Microsoft Graph output first. See the [sample file](sample-policies-for-review.json) for the format.
- Simulation does not cover device compliance, role conditions or device filter conditions. It treats risk-based policies as not applied.
- Use the results as reference information for reviewing your configuration (they are not official certification or assurance for any standard).

## Who it is for

Microsoft Entra ID administrators who design, review or report on Conditional Access

## Get the app

- [Microsoft Store](https://apps.microsoft.com/detail/9NR10PX75754)
- [Product site](https://capolanalyzer.sumikkolab.com/?lang=en) / [User manual](https://capolanalyzer.sumikkolab.com/manual/?lang=en) / [Support](https://capolanalyzer.sumikkolab.com/support.html)

The app is free to install with a 15-day trial from first launch. The trial does not include Pro features (simulation, Excel and PDF export). To keep using the app, buy the Standard or Pro add-on. See Microsoft Store for prices.

Requirements: Windows 10 version 2004 or later, or Windows 11 (x64), and WebView2 Runtime. The app is available in Japanese and English.
