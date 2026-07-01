# 📡 Estudo de APIs REST com Postman

Projeto prático desenvolvido para aprender e testar requisições HTTP em uma API pública, aplicando boas práticas de organização e validação de respostas.

---

## 🛠️ Ferramentas utilizadas
- **Postman**: Criação, envio e validação de requisições
- **JSONPlaceholder**: API pública gratuita e confiável para simulação de dados
- **GitHub**: Versionamento e compartilhamento do projeto

---

## ✅ Funcionalidades implementadas
Todos os principais métodos HTTP foram testados e validados:

| Método | Finalidade | O que faz |
|---|---|---|
| `GET` | Consultar dados | Lista todos os registros ou busca um item específico por ID |
| `POST` | Criar novo dado | Cadastra um novo registro na API |
| `PUT` | Atualização completa | Substitui **todos os campos** de um registro existente |
| `PATCH` | Atualização parcial | Altera **apenas os campos informados**, mantendo o resto dos dados |
| `DELETE` | Remoção | Exclui um registro (simulado nessa API de teste) |

---

## 🚀 Boas práticas aplicadas
✅ Uso de **variáveis** → `{{base_url}}` para reutilizar o endereço e manter a organização
✅ **Testes automáticos** → Verificam se o status e o conteúdo da resposta estão corretos
✅ Estrutura organizada → Nomes claros para cada requisição

---

## 📸 Exemplos de execução e resultados

> **1. Requisição GET - Listar todos os usuários**
> - URL: `{{base_url}}/users`
> - Resultado esperado: Status `200 OK` + lista de usuários em formato JSON

> **2. Requisição POST - Criar novo registro**
> - URL: `{{base_url}}/posts`
> - Corpo enviado:
> ```json
> {
>   "title": "Meu primeiro cadastro",
>   "body": "Aprendendo a usar o método POST no Postman",
>   "userId": 1
> }
> ```
> - Resultado: Status `201 Created` + retorno com o ID gerado automaticamente

> **3. Requisição PATCH - Alterar apenas um campo**
> - URL: `{{base_url}}/posts/1`
> - Enviado só o campo que quer mudar, mantendo o restante dos dados

---

## 📁 Arquivos disponíveis
- `Lab Postman - JSONPlaceholder.postman_collection.json`: Coleção completa, pronta para **importar diretamente no Postman**

---

## 📥 Como importar no Postman
1. Baixe o arquivo `.json` deste repositório
2. Abra o Postman → clique em **Import**
3. Selecione o arquivo → pronto, toda a estrutura será carregada
