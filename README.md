# Pet Lover

Bem-vindo ao **Pet Lover**, um sistema de gerenciamento para pet shops e clínicas veterinárias.

> **Este projeto foi desenvolvido como parte da disciplina de Programação Orientada a Objetos.**

O sistema permite o cadastro, listagem, atualização e exclusão de clientes, pets, produtos e serviços, além de registrar vendas e gerar relatórios de consumo.

## Índice

- [Funcionalidades](#funcionalidades)
- [Estrutura do Projeto](#estrutura-do-projeto)
- [Como Executar](#como-executar)
- [Como Usar](#como-usar)
- [Dependências](#dependências)
- [Detalhes Técnicos](#detalhes-técnicos)
- [Autores](#autores)

---

## Funcionalidades

- Cadastro, listagem, atualização e exclusão de:
  - Clientes
  - Pets
  - Produtos
  - Serviços
- Registro de vendas de produtos e serviços para clientes
- Relatórios:
  - Produtos e serviços mais consumidos
  - Clientes que mais consumiram em quantidade e valor
  - Consumo por tipo e/ou raça de pet
- Persistência de dados via arquivo JSON

---

## Estrutura do Projeto

```
.
├── src/
│   ├── app/
│   │   ├── cliente.json
│   │   └── main.ts
│   ├── io/
│   │   └── entrada.ts
│   ├── modelo/
│   │   ├── cliente.ts
│   │   ├── cpf.ts
│   │   ├── empresa.ts
│   │   ├── pet.ts
│   │   ├── produto.ts
│   │   ├── rg.ts
│   │   ├── servico.ts
│   │   └── telefone.ts
│   └── negocio/
│       ├── cadastro.ts
│       ├── cadastroCliente.ts
│       ├── cadastroPet.ts
│       ├── cadastroProduto.ts
│       ├── cadastroServico.ts
│       ├── listagem.ts
│       ├── listagemClientes.ts
│       ├── listagemPet.ts
│       ├── listagemProduto.ts
│       ├── listagemServico.ts
│       └── outros.ts
├── package.json
├── tsconfig.json
└── .gitignore
```

---

## Como Executar

1. **Clone o repositório:**
   ```sh
   git clone https://github.com/Agathawei070/T1.git
   cd T1
   ```

2. **Instale as dependências:**
   ```sh
   npm install
   ```

3. **Compile o projeto:**
   ```sh
   npx tsc
   ```

4. **Execute o sistema:**
   ```sh
   node out/app/main.js
   ```

---

## Como Usar

Ao iniciar o sistema, você verá um menu interativo no terminal com as opções:

- **Clientes:** Cadastrar, listar, atualizar e deletar clientes.
- **Pets:** Cadastrar, listar, buscar, editar e deletar pets de clientes.
- **Produtos e Serviços:** Gerenciar cadastro, listagem, edição e exclusão.
- **Vendas:** Registrar vendas de produtos e serviços para clientes.
- **Relatórios:** Visualizar consumo de produtos/serviços por clientes, por tipo/raça de pet, e os maiores consumidores.
- **Sair:** Encerra o sistema.

Basta digitar o número da opção desejada e seguir as instruções.

---

## Dependências

- [TypeScript](https://www.typescriptlang.org/)
- [prompt-sync](https://www.npmjs.com/package/prompt-sync)
- [@types/node](https://www.npmjs.com/package/@types/node)
- [@types/prompt-sync](https://www.npmjs.com/package/@types/prompt-sync)

---

## Detalhes Técnicos

- **Persistência:** Os dados são lidos e gravados no arquivo [`src/app/cliente.json`](src/app/cliente.json).
- **Organização:** O código está dividido em módulos para facilitar a manutenção e a escalabilidade.
- **Validações:** O sistema valida entradas de dados como datas, números e textos para evitar inconsistências.
- **Relatórios:** Diversos relatórios para análise de consumo e perfil dos clientes.

---

## Autores

- Desenvolvido por Agatha Wei

---

Sinta-se à vontade para contribuir, sugerir melhorias ou relatar problemas!
