# Terri Tracking Legal

Public, versioned policy documents for Terri Tracking, served by GitHub Pages at
<https://territechnologies.github.io/terri-legal/>. Terri GPS stores each URL as the
"Public Document URL" of a policy version.

## Rules

- **Never edit, rename or delete a published file.** Users accepted that exact file, and Terri GPS
  keeps its SHA-256 hash. A change always goes into a new version folder.
- **Publish only legally approved final PDFs.** This repository and its history are public, so
  drafts, review notes and placeholders must never be committed.
- **Upload the same file to Terri GPS.** The file chosen as "Approved Document File" must be
  byte-for-byte the file at the public URL.

## Layout

```
terms/v1.0/terms-and-conditions.pdf
acceptable-usage/v1.0/acceptable-usage-policy.pdf
privacy/v1.0/privacy-policy.pdf
ridge/participant-declaration/v1.0/participant-declaration.pdf
ridge/platform-terms-of-use/v1.0/platform-terms-of-use.pdf
ridge/refund-and-cancellation-policy/v1.0/refund-and-cancellation-policy.pdf
ridge/privacy-notice/v1.0/privacy-notice.pdf
```

## Publishing a new version

1. Export the approved document to PDF.
2. Copy it into a new folder, for example `privacy/v1.1/privacy-policy.pdf`.
3. Add the version, with `sha256sum` output, to `index.html` and mark it as current.
4. Commit, push, and wait for the Pages deployment to finish.
5. Download the public URL and check that its `sha256sum` matches the local file.
6. In Terri GPS, open Settings → Policies and publish the version with that URL and the same PDF,
   then check that the hash Terri GPS shows matches.
