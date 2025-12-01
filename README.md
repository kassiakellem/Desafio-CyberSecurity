<img width="2816" height="1536" alt="RelatorioFinal" src="https://github.com/user-attachments/assets/fca0c924-07e6-48cc-8fcf-8e99ce41f256" />


# 🛡️ Relatório Técnico de Pentest - CTF
# Desafio-CyberSecurity
Curso - Cyber Security Desafio de Final CTF 

> **Autor:** Kássia Kellem
> **Data:** Novembro/2025
> **Status:** Concluído 🚩

## 📋 Sobre o Projeto
Este repositório contém o relatório técnico detalhado e os artefatos de um Teste de Intrusão (Penetration Test) realizado em ambiente controlado (CTF - Capture The Flag).

O objetivo foi explorar vulnerabilidades em uma infraestrutura simulada da "TechCorp Laboratories", cobrindo desde a enumeração de serviços até a exploração avançada de falhas de execução remota de código (RCE).

## 🎯 Escopo e Alvos
* **Alvo 1 (Legado):** Servidor Web PHP/MySQL.
* **Alvo 2 (Moderno):** Aplicação em Microserviços (Node.js & Python/Flask).

## 🛠️ Ferramentas Utilizadas
* **Reconhecimento:** Nmap, Gobuster, Browser DevTools.
* **Exploração Web:** Burp Suite, Curl, SQLMap.
* **Scripts Customizados:** Python (Exploit de Desserialização), Bash.
* **Acesso:** SSH, FTP, Reverse Shells.

## 🚩 Principais Vulnerabilidades Identificadas
Durante a análise, foram capturadas **10 Flags**, explorando falhas críticas como:

1.  **RCE via Insecure Deserialization (Python Pickle):** Exploração de falha crítica na API (Porta 5000) permitindo execução de comandos como root.
2.  **RCE via File Upload (Node.js):** Injeção de comandos através de manipulação de nomes de arquivos na galeria de imagens (Porta 8000).
3.  **SQL Injection:** Extração completa do banco de dados no servidor legado.
4.  **Exposição de Credenciais:** Senhas *hardcoded* em arquivos fonte e vazamento via `robots.txt` e backups.
5.  **Configurações Inseguras:** FTP Anônimo e permissões de diretório incorretas.

## 📂 Estrutura do Repositório
* `/capturas`: Evidências visuais (screenshots) das vulnerabilidades e flags.
* `/scripts`: Exploits desenvolvidos durante o teste (ex: gerador de payload Pickle).
* `Relatorio-Tecnico.pdf`: Documento formal com a análise de impacto e sugestões de correção.

---
### ⚠️ Aviso Legal (Disclaimer)
Este projeto foi realizado para fins estritamente educacionais em ambiente de laboratório autorizado. O uso das técnicas descritas contra alvos sem consentimento prévio é ilegal.
