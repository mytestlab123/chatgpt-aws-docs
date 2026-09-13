# AWS Control Paths

There are two useful ways to work with AWS.

## Fast path

Use a connected AWS tool for live inspection, troubleshooting, comparison, experiments, and verification.

## Deterministic path

Use Git, infrastructure as code, and CI/CD for changes that should be retained, reviewed, repeated, and rebuilt later.

## Recommended loop

```text
inspect -> decide -> encode in Git/IaC -> deploy -> verify
```

Use the fast path to learn and diagnose. Use the deterministic path for long-lived delivery.

| Need | Preferred path |
|---|---|
| Inspect current state | Connected AWS tool |
| Troubleshoot | Connected AWS tool |
| Small reversible experiment | Connected AWS tool |
| Persistent infrastructure | Git + IaC |
| Repeatable deployment | Git + CI/CD |
| Independent verification | Connected AWS tool |
