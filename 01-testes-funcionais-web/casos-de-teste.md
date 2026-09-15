# 🧪 Casos de Teste - Login

## 📌 Funcionalidade

Autenticação de usuários na aplicação SauceDemo.

## CT-001 - Login com usuário e senha válidos

**Tipo:** Positivo

**Pré-condição:**  
Estar na página de login do SauceDemo e possuir credenciais válidas para autenticação.

**Dados de teste:**

- Usuário: `standard_user`
- Senha: `secret_sauce`

**Passos:**
1. Inserir o usuário `standard_user` no campo "Username".
2. Inserir a senha `secret_sauce` no campo "Password".
3. Clicar no botão "Login".

**Resultado esperado:**
O sistema deve autenticar o usuário com sucesso e direcioná-lo para a página de produtos.

---

## CT-002 - Login com usuário e senha inexistentes

**Tipo:** Negativo

**Pré-condição:**  
Estar na página de login do SauceDemo.

**Dados de teste:**

- Usuário: `usuario_inexistente`
- Senha: `senha_invalida`

**Passos:**

1. Inserir o usuário `usuario_inexistente` no campo "Username".
2. Inserir a senha `senha_invalida` no campo "Password".
3. Clicar no botão "Login".

**Resultado esperado:**  
O sistema não deve autenticar o usuário e deve apresentar uma mensagem informando que o usuário e a senha não correspondem a um usuário válido.

---

## CT-003 - Login informando apenas o usuário

**Tipo:** Negativo

**Pré-condição:**  
Estar na página de login do SauceDemo.

**Dados de teste:**

- Usuário: `standard_user`

**Passos:**

1. Inserir o usuário `standard_user` no campo "Username".
2. Não preencher o campo "Password".
3. Clicar no botão "Login".

**Resultado esperado:**  
O sistema não deve autenticar o usuário e deve apresentar uma mensagem informando que o campo "Password" é obrigatório.

---

## CT-004 - Login com usuário válido e senha inválida

**Tipo:** Negativo

**Pré-condição:**  
Estar na página de login do SauceDemo.

**Dados de teste:**

- Usuário: `standard_user`
- Senha: `invalid_password`

**Passos:**

1. Inserir o usuário `standard_user` no campo "Username".
2. Inserir a senha `invalid_password` no campo "Password".
3. Clicar no botão "Login".

**Resultado esperado:**  
O sistema não deve autenticar o usuário e deve apresentar uma mensagem informando que as credenciais fornecidas são inválidas.

----

## CT-005 - Login com usuário inválido e senha válida

**Tipo:** Negativo

**Pré-condição:**  
Estar na página de login do SauceDemo.

**Dados de teste:**

- Usuário: `usuario_inexistente`
- Senha: `secret_sauce`

**Passos:**

1. Inserir o usuário `usuario_inexistente` no campo "Username".
2. Inserir a senha `secret_sauce` no campo "Password".
3. Clicar no botão "Login".

**Resultado esperado:**  
O sistema não deve autenticar o usuário e deve apresentar uma mensagem informando que as credenciais fornecidas são inválidas.

---
## CT-006 - Login informando apenas a senha

**Tipo:** Negativo

**Pré-condição:**  
Estar na página de login do SauceDemo.

**Dados de teste:**

- Senha: `secret_sauce`

**Passos:**

1. Não preencher o campo "Username".
2. Inserir a senha `secret_sauce` no campo "Password".
3. Clicar no botão "Login".

**Resultado esperado:**  
O sistema não deve autenticar o usuário e deve apresentar uma mensagem informando que o campo "Username" é obrigatório.

---

## CT-007 - Login sem informar usuário e senha

**Tipo:** Negativo

**Pré-condição:**  
Estar na página de login do SauceDemo.

**Dados de teste:**

- Não se aplica.

**Passos:**

1. Não preencher o campo "Username".
2. Não preencher o campo "Password".
3. Clicar no botão "Login".

**Resultado esperado:**  
O sistema não deve autenticar o usuário e deve apresentar mensagem de validação referente aos campos obrigatórios não preenchidos.

---

## CT-008 - Login com usuário bloqueado

**Tipo:** Negativo

**Pré-condição:**  
Estar na página de login do SauceDemo.

**Dados de teste:**

- Usuário: `locked_out_user`
- Senha: `secret_sauce`

**Passos:**

1. Inserir o usuário `locked_out_user` no campo "Username".
2. Inserir a senha `secret_sauce` no campo "Password".
3. Clicar no botão "Login".

**Resultado esperado:**  
O sistema não deve autenticar o usuário e deve apresentar uma mensagem informando que o usuário está bloqueado.
