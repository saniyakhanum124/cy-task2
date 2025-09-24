# Phishing Email Analysis Report

## 1️⃣ Sample

-   File analyzed: **PhishingSample.EML.txt**\
-   Content: Marketing-style email promoting **"KetoXplode" weight loss
    gummies**, mostly in German.

## 2️⃣ Sender Address (Spoofing Check)

-   **From:** Magisches Schlankheitssystem🤸‍♀️✅
    <otto-newsletter@newsletter.otto.de>\
-   **Return-Path / Reply-To:** return@winner-win.art /
    reply_to@winner-win.art\
-   **Suspicious:**
    -   Pretends to be "Otto Newsletter" (a legitimate retailer)\
    -   Actual domain is `winner-win.art` --- unrelated to Otto.\
    -   Classic spoofing.

## 3️⃣ Email Header Discrepancies

-   **SPF:** softfail --- "domain of transitioning winner-win.art
    discourages use of 80.96.157.90 as permitted sender."\
-   **DKIM:** none (not signed).\
-   **DMARC:** fail.\
-   **Originating IP:** 80.96.157.90 (not Otto or Microsoft).\
-   **Microsoft Spam Score:** SCL:7 and BCL:8 --- very high spam/phish
    likelihood.

## 4️⃣ Suspicious Links / Attachments

Extracted URLs: - hxxps://t\[.\]co/eYVtqVunRC\
- hxxp://bsq2\[.\]firiri\[.\]shop/... (multiple variations)\
- Hidden tracker: hxxp://bsq2\[.\]firiri\[.\]shop/RStjU3...

⚠️ No attachments, but the links are unsafe.

## 5️⃣ Urgent / Threatening Language

-   "Beeilen Sie sich!" ("Hurry up!")
-   "Extrem hohe Nachfrage" ("extremely high demand")
-   Uses scarcity and urgency to trick users.

## 6️⃣ Mismatched URLs

-   Display text suggests a known brand "Otto" but hover links actually
    point to t.co shortener → redirects to unknown firiri.shop.
-   Clear mismatch between visible brand and real destination.

## 7️⃣ Spelling / Grammar

-   Mostly grammatically correct German.
-   Spammy formatting: all-caps, emojis, flashy text.

## 8️⃣ Summary of Phishing Traits

-   Spoofed sender pretending to be Otto.
-   Failed SPF/DKIM/DMARC authentication.
-   Suspicious shortened/obfuscated links (t.co + unknown .shop domain).
-   Urgency and miracle weight loss product (common scam).
-   Hidden tracking pixels.
-   High spam score (SCL:7).

## ✅ Conclusion

This email is a phishing/spam campaign to lure users to click a
shortened link leading to fraudulent pages.\
**Action:** Mark as spam, block the domain, and do NOT click links.
