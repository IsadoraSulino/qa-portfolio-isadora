# 🧪 Cenários de Teste - Login

## 📌 Funcionalidade

Autenticação de usuários na aplicação SauceDemo.

## 🎯 Objetivo

Validar o comportamento da funcionalidade de login em diferentes condições, contemplando cenários positivos e negativos.

## 📋 Cenários de Teste

| ID | Cenário | Tipo |
|---|---|---|
| CT-001 | Validar login com usuário e senha válidos | Positivo |
| CT-002 | Validar login com usuário e senha inexistentes | Negativo|
| CT-003 | Validar login informando apenas o usuário | Negativo|
| CT-004 | Validar login com usuário válido e senha inválida| Negativo|
| CT-005 | Validar login com usuário inválido e senha válida | Negativo|
| CT-006 | Validar login informando apenas a senha | Negativo|
| CT-007 | Validar login sem informar usuário e senha | Negativo |
| CT-008 | Validar login com usuário bloqueado | Negativo |
