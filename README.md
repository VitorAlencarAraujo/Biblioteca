# Biblioteca

Projeto acadêmico desenvolvido para a atividade de Banco de Dados (BCD), com o objetivo de planejar, implementar e consultar um banco de dados relacional para o gerenciamento de uma biblioteca.

## Demonstração

Acesse o site do projeto: [Biblioteca — Vercel](https://biblioteca-biblioteca.vercel.app/#projeto)

## Objetivos

- Modelar um banco de dados relacional para uma biblioteca.
- Implementar tabelas, chaves primárias e chaves estrangeiras.
- Aplicar conceitos de normalização de dados.
- Desenvolver consultas SQL para recuperar e analisar informações.
- Documentar o projeto e disponibilizar sua apresentação na web.

## Tecnologias utilizadas

- **MySQL** — criação e gerenciamento do banco de dados.
- **SQL** — definição das tabelas, relacionamentos e consultas.
- **HTML5** — estruturação do site.
- **CSS3** — estilização e responsividade da interface.
- **Git e GitHub** — versionamento e armazenamento do código.
- **Vercel** — hospedagem do site.

## Modelo do banco de dados

O banco de dados `BibliotecaDB` é composto por quatro tabelas principais:

| Tabela | Descrição |
|---|---|
| `Usuarios` | Armazena os dados dos usuários da biblioteca. |
| `Autores` | Armazena os dados dos autores das obras. |
| `Livros` | Registra os livros, suas categorias, anos de publicação e autores. |
| `Emprestimos` | Registra os empréstimos realizados pelos usuários e as datas correspondentes. |

### Relacionamentos

- **Autores → Livros:** um autor pode estar relacionado a vários livros.
- **Usuarios → Emprestimos:** um usuário pode realizar vários empréstimos.
- **Livros → Emprestimos:** um livro pode aparecer em vários registros de empréstimo ao longo do tempo.

As relações são implementadas com chaves estrangeiras para manter a integridade referencial dos dados.

## Normalização

O projeto aborda as formas normais de banco de dados:

- **1FN — Primeira Forma Normal:** organização dos dados em valores atômicos, sem grupos repetitivos.
- **2FN — Segunda Forma Normal:** eliminação de dependências parciais em relação às chaves candidatas.
- **3FN — Terceira Forma Normal:** redução de dependências transitivas entre atributos não chave.
- **4FN — Quarta Forma Normal:** análise de dependências multivaloradas independentes.

A aplicação dessas formas normais contribui para reduzir redundâncias e melhorar a consistência dos dados.

## Consultas SQL

O projeto contempla consultas para explorar os dados armazenados, incluindo:

- Consultas com `SELECT`, `WHERE` e `ORDER BY`.
- Filtragem de registros com `LIKE`, `BETWEEN` e verificações de valores nulos.
- Junções entre tabelas utilizando `JOIN`.
- Agrupamento e agregação de dados com `GROUP BY` e funções agregadoras.

## Estrutura do projeto

```text
Biblioteca/
├── Biblioteca/
│   ├── index.html
│   └── style.css
└── README.md
```

## Como executar

1. Clone o repositório:

   ```bash
   git clone https://github.com/VitorAlencarAraujo/Biblioteca.git
   ```

2. Entre na pasta do projeto:

   ```bash
   cd Biblioteca
   ```

3. Abra a pasta interna `Biblioteca` e execute o arquivo `index.html` em seu navegador.

O site é estático e utiliza HTML e CSS, portanto não exige um servidor de aplicação para ser visualizado localmente.

## Banco de dados e hospedagem

O banco de dados é desenvolvido em MySQL. A hospedagem em nuvem e a geração de um arquivo de backup (`dump`) fazem parte das etapas de entrega previstas para a atividade.

**Observação:** o site publicado apresenta a documentação visual do projeto. Ele não estabelece, por si só, uma conexão direta com o banco de dados MySQL.

## Autor

**Vitor Alencar Araujo**

Estudante de Desenvolvimento de Sistemas — SENAI.

---

Projeto desenvolvido para fins acadêmicos na atividade de Banco de Dados (BCD).
