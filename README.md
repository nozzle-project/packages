# packages
Minimal CLI for infrastructure automation using Python-like scripts.

# 🔐 Hardening SSH com Nozzle

Este pacote aplica uma configuração segura no serviço SSH em um host remoto, garantindo que o acesso root direto seja desativado (`PermitRootLogin no`).

## ✔️ O que faz

- Edita o arquivo `/etc/ssh/sshd_config`
- Garante que `PermitRootLogin no` esteja definido
- Reinicia o serviço `sshd` se houver alterações

## 📦 Requisitos

- Acesso SSH com sudo sem senha (NOPASSWD)
- Nozzle instalado no controlador

## 🚀 Como usar

```bash
nozzle ssh_hardening.nzl

