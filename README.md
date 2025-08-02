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

# Nozzle v0.1.6

O **Nozzle** é uma ferramenta de automação simples, segura e poderosa com sintaxe inspirada em Python e JavaScript. Ideal para quem deseja criar playbooks leves e scripts reutilizáveis para administração de servidores.

---

## 📦 Conteúdo do pacote

- `nozzle` – binário executável da ferramenta
- `install-nozzle.sh` – script de instalação automatizado

---

## 🚀 Instalação

### 1. Baixe e extraia o pacote:

```bash
wget https://github.com/nozzle-project/packages/releases/download/v0.1.6/nozzle-0.1.6.tar.gz
tar -xzf nozzle-0.1.6.tar.gz
cd nozzle-0.1.6
```

### 2. Execute o instalador:

```bash
./install-nozzle.sh
```

Isso copiará o binário para `/usr/local/bin/nozzle` com as permissões corretas.

---

## ✅ Testando

Após a instalação, execute:

```bash
nozzle --version
```

Ou execute um script `.nzl`:

```bash
nozzle meu-playbook.nzl
```

---

## 🧠 Recursos principais

- Execução local e remota de comandos (`sh`, `ssh`)
- Transferência de arquivos via `scp`
- Templates com `tpl`
- Edição de arquivos com `replace_line`
- Execução paralela com `parallel_for`
- JSON helpers
- Modo `--dry-run` para simulações

---

## 🔒 Requisitos

- Linux/macOS
- Python 3.4+
- `ssh`, `scp` e `sudo` disponíveis no sistema

---

## 📚 Documentação

Acesse: [https://nozzle-project.github.io](https://nozzle-project.github.io)

---

## 💬 Comunidade

- [Página da Comunidade](https://nozzle-project.github.io/community)
- Reporte bugs ou contribua: [https://github.com/nozzle-project](https://github.com/nozzle-project)

---

## 🧾 Licença

MIT © 2025 Nozzle Project
