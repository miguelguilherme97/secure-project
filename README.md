# 🔐 Secure PR Validator

Mini ferramenta de validação de código desenvolvida em **Python** para simular um **Security Quality Gate** em pipelines de CI/CD.

Este projeto foi criado como laboratório prático para estudo de **DevSecOps**, automação e análise estática de código.

---

## 🚀 Objetivo

Simular o funcionamento básico de uma ferramenta de:

- 🔎 Static Code Analysis (SAST)
- 🔐 Policy as Code
- 🚦 Security Gate em CI/CD
- 🛑 Bloqueio automático de Pull Request

O script analisa arquivos `.py` do projeto e falha a execução caso encontre padrões inseguros.

---

## 🛠️ Regras Implementadas

O validator atualmente detecta:

- ❌ Uso de `print()` em código
- ❌ Presença de `TODO`
- ❌ Senhas hardcoded (ex: `password = "123"`)

Se algum desses padrões for encontrado:

- O script exibe os erros encontrados
- Mostra o total de problemas
- Retorna `exit code 1`
- Simula falha de pipeline
