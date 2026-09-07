# Outreach Response Ledger

A daily report of what ChatDaddy's churn win-back and onboarding activation
campaigns actually sent, who answered, whether a human answered them, and who
went on to pay.

**This repository is public and holds no readable data.** `data.enc.json` is
AES-256-GCM ciphertext; the page derives the key from `?key=…` with PBKDF2 and
decrypts it in your browser. Without the key it is 42KB of noise.

Open it with the key appended:

```
https://ahay45.github.io/chatdaddy-outreach-ledger/?key=…
```

The report is rebuilt and re-encrypted daily by a private workflow that holds
the credentials — this repo only ever receives the finished, encrypted file.
Source for the build lives in `chatdaddy/p0-recovery-agent` under
`outreach-ledger/`.
