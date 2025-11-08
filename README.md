````markdown
<!-- README.md -->

_____________________________________________________________________
  _____ _____ ______   ______ _    _ _  __ _  __  __  _  __  _  ____
 |  __ \_   _|  ____| |  ____| |  | | |/ /| |/ / | ||  \/  |/ __ \
 | |  | || | | |__    | |__  | |  | | ' / | ' /  | || \  / | |  | |
 | |  | || | |  __|   |  __| | |  | |  <  |  <   | || |\/| | |  | |
 | |__| || |_| |____  | |____| |__| | . \ | . \ _| || |  | | |__| |
 |_____/_____|______| |______|\____/|_|\_\|_|\_(_)_||_|  |_|\____/
_____________________________________________________________________

# JEFF H4CK — Cybersecurity Underground

![Linux](https://img.shields.io/badge/Linux-%2326272b.svg?style=for-the-badge&logo=linux&logoColor=white)
![Python](https://img.shields.io/badge/Python-%233776AB.svg?style=for-the-badge&logo=python&logoColor=white)
![Kali](https://img.shields.io/badge/Kali-%23007ACC.svg?style=for-the-badge&logo=kali-linux&logoColor=white)
![Offense](https://img.shields.io/badge/Offense-%23ff3b65.svg?style=for-the-badge)
![RAG+n8n](https://img.shields.io/badge/RAG--n8n-%2300ff9f.svg?style=for-the-badge)

---

> SIGIL: `JEFF H4CK`  
> ETHIC: testes autorizados — nada ilegal.

---

## Sobre
Especialista em **pentest**, **engenharia reversa**, **cryptohandling** e **automação IA**. Root no terminal, olhos no tráfego, mente no exploit chain.

---

## Skills
- Recon & OSINT — nmap, shodan, recon-ng, amass  
- Web Exploitation — RCE, SQLi, XSS, auth bypass  
- Binary & Mobile — análise estática/dinâmica, APKs, PFX handling  
- Infra & Ops — hardening Linux, containers, CI/CD abuse  
- Automação — n8n, RAG (Supabase/Postgres), agents para triagem

---

## Toolset
```bash
# ambiente rápido
sudo apt update && sudo apt install -y nmap git python3 python3-pip jq
git clone git@github.com:JEFFH4CK/cyber-lab.git
cd cyber-lab && ./run-recon.sh
````

---

## Projetos

* Pentest Reports — PoC, screenshots, mitigations.
* RAG + n8n — indexador de PDFs/TXT/CSV -> vetores -> agente Q&A.
* Agent Triager — pré-análise de alertas, geração automática de tickets.

---

## Arte & Banner (salvar arquivos conforme indicado)

### 1) ASCII banner (use como header)

```text
# arquivo: ASCII_BANNER.txt
  _____ _____ ______   ______ _    _ _  __ _  __  __  _  __  _  ____
 |  __ \_   _|  ____| |  ____| |  | | |/ /| |/ / | ||  \/  |/ __ \
 | |  | || | | |__    | |__  | |  | | ' / | ' /  | || \  / | |  | |
 | |  | || | |  __|   |  __| | |  | |  <  |  <   | || |\/| | |  | |
 | |__| || |_| |____  | |____| |__| | . \ | . \ _| || |  | | |__| |
 |_____/_____|______| |______|\____/|_|\_\|_|\_(_)_||_|  |_|\____/
                           JEFF H4CK
```

### 2) Shell animation script

```bash
# arquivo: anim_ascii.sh
# execução: bash anim_ascii.sh
#!/usr/bin/env bash
cols=$(tput cols 2>/dev/null || echo 80)
frames=(
"⣾ JEFF H4CK — SNIFF & PWN"
"⣽ JEFF H4CK — SNIFF & PWN"
"⣻ JEFF H4CK — SNIFF & PWN"
"⢿ JEFF H4CK — SNIFF & PWN"
"⡿ JEFF H4CK — SNIFF & PWN"
"⣟ JEFF H4CK — SNIFF & PWN"
"⣯ JEFF H4CK — SNIFF & PWN"
"⣷ JEFF H4CK — SNIFF & PWN"
)
clear
while true; do
  for f in "${frames[@]}"; do
    printf "\r%s" "$(printf '%*s' $(( (cols - ${#f})/2 )) '')$f"
    sleep 0.09
  done
done
```

### 3) SVG glitch banner

```svg
<!-- arquivo: banner_glitch.svg -->
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 900 200" width="900" height="200">
  <defs>
    <filter id="g">
      <feTurbulence baseFrequency="0.015 0.25" numOctaves="1" seed="7" result="t"/>
      <feDisplacementMap in="SourceGraphic" in2="t" scale="12" xChannelSelector="R" yChannelSelector="G"/>
    </filter>
    <linearGradient id="g1" x1="0" x2="1">
      <stop offset="0" stop-color="#00ff9f"/>
      <stop offset="1" stop-color="#00a9ff"/>
    </linearGradient>
    <style><![CDATA[
      .bg { fill: #030303; }
      .txt { font: 84px 'Courier New', monospace; font-weight:800; fill:url(#g1); letter-spacing:6px; }
      .sub { font:14px monospace; fill:#8a8f95; }
    ]]></style>
  </defs>

  <rect class="bg" width="100%" height="100%"/>
  <g filter="url(#g)">
    <text x="50%" y="56%" text-anchor="middle" class="txt">JEFF H4CK</text>
  </g>
  <text x="50%" y="78%" text-anchor="middle" class="sub">Cybersecurity · Pentest · Automation</text>
</svg>
```

### 4) HTML animated banner

```html
<!-- arquivo: banner.html -->
<!doctype html>
<html lang="pt-BR">
<head>
<meta charset="utf-8"/>
<meta name="viewport" content="width=device-width,initial-scale=1"/>
<title>JEFF H4CK</title>
<style>
  html,body{height:100%;margin:0;background:#010101;color:#a6f0d1;font-family:ui-monospace, SFMono-Regular, Menlo, "Courier New", monospace;display:flex;align-items:center;justify-content:center}
  .box{width:880px;max-width:94%;padding:28px;border-radius:10px;border:1px solid rgba(255,255,255,0.04);background:linear-gradient(180deg, rgba(0,0,0,0.6), rgba(0,0,0,0.45));box-shadow:0 12px 40px rgba(0,0,0,0.7)}
  .title{font-size:54px;letter-spacing:8px;margin:0;color:#00ff9f}
  .tag{margin-top:6px;font-size:13px;color:#8a8f95}
  .scan{margin-top:18px;height:8px;background:#071;overflow:hidden;border-radius:8px;position:relative}
  .bar{position:absolute;left:-30%;width:30%;height:100%;background:linear-gradient(90deg,transparent,#00ff9f,transparent);animation:scan 1.6s linear infinite}
  @keyframes scan{0%{left:-30%}100%{left:130%}}
  .glitch{position:absolute;inset:0;mix-blend-mode:screen;pointer-events:none;opacity:0.08;background:
    repeating-linear-gradient(0deg, rgba(255,255,255,0.02) 0px, rgba(255,255,255,0.01) 2px);filter:blur(2px)}
</style>
</head>
<body>
  <div class="box">
    <div class="glitch"></div>
    <h1 class="title">JEFF H4CK</h1>
    <div class="tag">Cybersecurity · Pentest · Automation</div>
    <div class="scan"><div class="bar"></div></div>
  </div>
</body>
</html>
```

---

## Contato

* GitHub: `https://github.com/JEFFH4CK`
* Email: `jeffh4ck@alphatrix.ai`

---

## Nota final

Testes somente com autorização. Use com responsabilidade.

```
```
