# heron

heron is a small phishing triage tool. It reads a folder of `.eml` files,
parses each email, checks it against a set of suspicious indicators and
adds up a score. Based on that score, every email gets a verdict:
**benign**, **suspicious** or **phishing**.

The sample emails in `data/samples` are synthetic: they use reserved
domains and IP addresses (`example`, `192.0.2.x`) that belong to nobody.

## How to run it

    python3 triage.py

The verdicts are written to `results.txt`.
