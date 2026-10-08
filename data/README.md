# Dataset Guide

Inventory recorded at: 2026-10-08T14:19:14+00:00
Exact download timestamps were not recorded.

## SpamAssassin Normal Email Candidates

- Provider: Apache SpamAssassin Public Corpus
- Source: https://spamassassin.apache.org/old/publiccorpus/
- File: 20030228_easy_ham.tar.bz2
- Download URL: https://spamassassin.apache.org/old/publiccorpus/20030228_easy_ham.tar.bz2
- Original label: ham (non-spam)
- Proposed project label: legitimate, pending content review
- Email count before deduplication: 2500
- Format: Individual raw email files
- Archive location: data/raw/spamassassin/20030228_easy_ham.tar.bz2
- Extracted location: data/raw/spamassassin/easy_ham/
- Archive SHA-256: 2b7b65904bcfcc31d2b5f51946f2d261370b257402cbbd62930b46ab83367438
- Source documentation: data/raw/spamassassin/source_readme.html
- Usage conditions: Offered for spam-filter testing.
  Copyright in message text remains with the original senders.
  Do not send corpus messages through live email systems.
- Raw messages will not be redistributed in this repository.

## Nazario Phishing Emails

- Provider: Jose Nazario
- Source: https://monkey.org/~jose/phishing/
- File: phishing0.mbox
- Download URL: https://monkey.org/~jose/phishing/phishing0.mbox
- Original label: Hand-classified phishing
- Proposed project label: phishing
- Email count before deduplication: 414
- Format: mbox containing multiple emails
- Local location: data/raw/nazario/phishing0.mbox
- File size in bytes: 3119972
- SHA-256: 6184b0a34ed8cbbb252676e21c1eab9eac5fa4be89c61e30cc9954ebbb25d848
- License: CC BY 4.0; attribution required
- Attribution: Nazario Phishing Corpus by Jose Nazario
- Source documentation: data/raw/nazario/source_README.txt
- License document: data/raw/nazario/source_LICENSE.txt
- Raw messages will not be redistributed in this repository.

## Limitations and Planned Checks

- These are historical datasets, not a current deployment benchmark.
- Ham means non-spam; it is not an explicit non-phishing annotation.
- Hand-classified labels may contain errors.
- The two classes come from different sources.
  A model may learn source-specific artifacts instead of phishing signals.
- Remove duplicates before creating training and test splits.
- Review class balance, parsing errors, and label quality.
- Keep source identifiers for each email during preprocessing.
- Do not use this two-source setup alone to claim cross-source robustness.

## Integrity Note

These hashes identify the locally downloaded files.
They have not been checked against publisher-provided checksums.

## Storage Policy

Raw emails, processed datasets, and downloaded source documents
remain outside Git. Only this guide is tracked.
