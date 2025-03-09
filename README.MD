Aqui está o código principal atualizado com a nova estrutura de pastas:

```markdown
# Documentação da API - MegaMan Bosses

## Visão Geral

Este projeto é uma API desenvolvida em [.NET Core 3.1](https://dotnet.microsoft.com/download/dotnet/3.1) para listar dados dos bosses da franquia MegaMan. A API fornece os dados em formato JSON conforme o exemplo abaixo:

```json
{
    "Id": 1,
    "Code": "DLN/DRN-003",
    "Name": "Cutman",
    "HP": 150,
    "Picture": "https://vignette.wikia.nocookie.net/megaman/images/2/22/Cutman.png"
}
```

---

## Tecnologias Utilizadas

| Tecnologia                                                                    | Versão | Link                                   |
| ----------------------------------------------------------------------------- | ------ | -------------------------------------- |
| [.NET Core](https://dotnet.microsoft.com/download/dotnet/3.1)                 | 3.1    | Framework principal para a API         |
| [Entity Framework Core](https://docs.microsoft.com/en-us/ef/core/)            | 3.1.8  | ORM para manipulação do banco de dados |
| [SQL Server](https://www.microsoft.com/pt-br/sql-server/sql-server-downloads) | -      | Banco de dados utilizado               |
| [Newtonsoft.Json](https://www.newtonsoft.com/json)                            | 12.0.2 | Biblioteca para manipulação de JSON    |

---

## Estrutura do Projeto

```
/src
├── .vs
│   └── MegamanApi
│       └── v15
├── .vscode
├── bin
│   └── Debug
│       └── netcoreapp3.1
│           └── Properties
│           └── runtimes
│               └── unix
│                   └── lib
│                       └── netcoreapp2.0
│                       └── netcoreapp2.1
│               └── win
│                   └── lib
│                       └── netcoreapp2.0
│                       └── netcoreapp2.1
│                       └── netstandard2.0
│               └── win-arm64
│                   └── native
│               └── win-x64
│                   └── native
│               └── win-x86
│                   └── native
├── Controllers
├── Database
│   ├── DTOs
│   │   └── Robots
│   ├── EntityFramework
│   │   ├── Context
│   │   └── Migrations
│   └── Repositories
│       └── Robots
├── middlewares
├── Models
├── obj
│   └── Debug
│       └── netcoreapp3.1
│           └── staticwebassets
├── Properties
├── Services
│   └── Robots
└── _docs
    └── assets
```

---

## Arquitetura do Projeto

![Arquitetura do Projeto](./_docs/architecture.png)

---

## Técnicas Utilizadas

- Injeção de dependência
- Utilização de DTOs para transferência segura de dados
- Organização por camadas para melhor manutenção do código

---

## Endpoints da API

### **GET /api/v1/robots**

- **Descrição:** Retorna a lista completa dos robôs.

### **GET /api/v1/robots/{id}**

- **Descrição:** Retorna um robô específico pelo seu `id`.

### **POST /api/v1/robots**

- **Descrição:** Envia um novo robô para a base de dados.

---

## Estrutura do Modelo `Robot`

```csharp
public class Robot
{
    public int Id { get; set; }
    public string Code { get; set; }
    public string Name { get; set; }
    public int HP { get; set; }
    public string Picture { get; set; }
}
```

---

## Contato

RobsonAndrade [GitHub](https://github.com/rdandrade2)
