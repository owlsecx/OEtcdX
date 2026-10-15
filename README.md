# 🦉 OEtcdX

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Linux-0a0c10?style=flat-square"/>
  <img src="https://img.shields.io/badge/Category-OScan-blue?style=flat-square"/>
  <img src="https://img.shields.io/badge/License-MIT-green?style=flat-square"/>
  <img src="https://img.shields.io/badge/Part%20of-OwlSec%20Toolkit-7b5ea7?style=flat-square"/>
  <img src="https://img.shields.io/badge/Version-1.0.0-cyan?style=flat-square"/>
</p>

> **OEtcdX** — etcd Key-Value Store Configuration Auditor

---

> ⚠️ **AUTHORISED USE ONLY** — Use only on systems you own or have explicit written permission to test. Unauthorised use is illegal.

---

## 📌 Overview

Offline read-only etcd configuration, RBAC, encryption-at-rest and snapshot security auditor

---

## ✨ Features

- Stdlib YAML subset parser; etcd.conf.yml, ETCD_* env, systemd ExecStart flags, static-pod etcd.yaml args
- Client & peer transport — http, 0.0.0.0, client-cert- auth, auto-tls, trusted CA, CN allow-list, ciphers
- etcdctl auth status / user list / user get / role get exports — auth disabled, password-less root, guest RW
- Kubernetes EncryptionConfiguration & kube-apiserver → etcd link: identity provider, missing secrets, keys
- pprof, debug logging, public metrics, v2 API, CORS, unsafe-no-fsync, force-new-cluster, experimental flags
- data-dir 0700, WAL / db / snapshot backups, key perms
- Secrets masked; --root mapping; CWE + MITRE ATT&CK
- TXT / MD / JSON / CSV / SARIF, --demo, --fail-on gates

---

## ⚙️ Requirements

- **Linux**
- **No Python installation needed** — runs as a standalone executable

---

## 🚀 Usage

```bash
./OEtcdX
```

---

## 📦 Part of OwlSec Toolkit

This tool is part of the **OwlSec** suite — a collection of 300+ security and privacy tools.

🔗 [owlsec.org](https://owlsec.org)

---

## ©️ License

MIT License — © Khaled S. Haddad

*Tools are distributed as pre-built executables. Source code is proprietary.*
