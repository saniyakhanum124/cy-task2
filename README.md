# cy-task2
# Phishing Email Analysis

## Project Overview

This repository contains an analysis of a **phishing email sample** to
demonstrate how to identify common phishing characteristics.

## Files in This Repository

-   **PhishingSample.EML.txt** -- Raw phishing email source (headers +
    body) used for analysis.
-   **phishing-analysis.md** -- Detailed analysis of the phishing email
    including spoofing detection, header checks, and phishing
    indicators.
-   **extracted_urls.txt** -- List of suspicious URLs extracted from the
    email (sanitized to prevent accidental clicks).

##  Steps Performed

1.  **Obtained Sample**\
    Used a publicly available phishing email sample
    (`PhishingSample.EML.txt`).
2.  **Sender Verification**\
    Checked `From`, `Reply-To`, and `Return-Path` headers for spoofing.
4.  **Header Analysis**\
    Verified SPF, DKIM, DMARC authentication results.
5.  **Link Extraction**\
    Extracted and sanitized suspicious URLs.
6.  **Content Review**\
    Looked for urgency, mismatched URLs, and grammar or formatting
    issues.
7.  **Summary**\
    Documented all phishing traits in `phishing-analysis.md`.

##  Key Findings

-   **Spoofed Sender**: Pretending to be a legitimate brand (Otto
    Newsletter) but actually from a suspicious domain
    (`winner-win.art`).
-   **Authentication Failures**: SPF softfail, DKIM missing, DMARC fail.
-   **Suspicious URLs**: Shortened redirect links leading to unknown
    domains.
-   **Urgent Language & Scam Content**: "Hurry up!", miracle weight loss
    claims.

## Recommendations

-   Never click suspicious links or open attachments from unknown
    senders.
-   Verify the sender's domain carefully.
-   Check email headers for SPF/DKIM/DMARC failures.
-   Report such emails to your email provider's abuse/phishing team.

## Pro Tip: 5-Second Check

Open the email source →
Search (Ctrl+F) for spf= or dmarc=.
If you see fail/softfail = immediate red flag.

