# 🦉 OEtcdX

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Linux-0a0c10?style=flat-square"/>
  <img src="https://img.shields.io/badge/Category-OScan-blue?style=flat-square"/>
  <img src="https://img.shields.io/badge/License-Proprietary-orange?style=flat-square"/>
  <img src="https://img.shields.io/badge/Part%20of-OwlSec%20Toolkit-7b5ea7?style=flat-square"/>
  <img src="https://img.shields.io/badge/Version-1.0.0-cyan?style=flat-square"/>
</p>

> **OEtcdX** — etcd Key-Value Store Configuration Auditor

---

> ⚠️ **AUTHORISED USE ONLY** — Use only on systems you own or have explicit written permission to test. Unauthorised use is illegal.

---

## 📌 Overview

OEtcdX — etcd Key-Value Store Configuration Auditor. It provides stdlib YAML subset parser; etcd.conf.yml, ETCD_* env, systemd ExecStart flags, static-pod etcd.yaml args; Client & peer transport — http, 0.0.0.0, client-cert- auth, auto-tls, trusted CA, CN allow-list, ciphers. Built-in demo/self-test paths and severity gates help validate detections without touching production when those flags are used.

---

## ✨ Features

- Stdlib YAML subset parser; etcd.conf.yml, ETCD_* env, systemd ExecStart flags, static-pod etcd.yaml args
- Client & peer transport — http, 0.0.0.0, client-cert- auth, auto-tls, trusted CA, CN allow-list, ciphers
- etcdctl auth status / user list / user get / role get exports — auth disabled, password-less root, guest RW
- Kubernetes EncryptionConfiguration & kube-apiserver → etcd link: identity provider, missing secrets, keys
- pprof, debug logging, public metrics, v2 API, CORS, unsafe-no-fsync, force-new-cluster, experimental flags
- data-dir 0700, WAL / db / snapshot backups, key perms

---

## ⚙️ Requirements

- **Linux**
- **No Python installation needed** — runs as a standalone executable

---

## 🚀 Usage

```bash
./OEtcdX <paths>
./OEtcdX <paths> --
./OEtcdX <paths> --root
./OEtcdX --help
```

---

## 📦 Part of OwlSec Toolkit

This tool is part of the **OwlSec** suite — a collection of 275+ security and privacy tools.

🔗 [owlsec.org](https://owlsec.org)

---

## ©️ License

Proprietary — © 2026 Owlsec LLC. All rights reserved.

*Tools are distributed as pre-built executables. Source code is proprietary.*

---

## 🔍 Verification & Transparency

This tool is closed-source. These files let you see exactly what is inside it,
without the source:

- [`SBOM.cdx.json`](SBOM.cdx.json) — CycloneDX inventory: SHA-256 of this
  binary, bundled CPython version, and every bundled library with its exact
  version and license. Feed it to Grype, Trivy or Dependency-Track to audit
  our dependencies for CVEs yourself.
- [`THIRD-PARTY-NOTICES.md`](THIRD-PARTY-NOTICES.md) — the full license text
  of every third-party component, extracted from this binary.

**No telemetry, no analytics, no licence check-in.** This tool does not phone
home. Verify that claim yourself:

```bash
sudo strace -f -e trace=network ./OEtcdX --help   # watch every network call
firejail --net=none ./OEtcdX --help               # deny the network entirely
```

Release signing, GPL compliance and vulnerability reporting:
[**TRUST.md**](https://github.com/owlsecx/owl-os/blob/main/TRUST.md)
