# 🗄️ Operações de Banco de Dados (MySQL)

Este guia resume as operações essenciais para **criação, listagem, alteração e exclusão** de bancos de dados e tabelas no MySQL.  
Pronto para estudo e aplicação prática.

---

## 🎯 Comandos Essenciais

### 🔹 Conectar ao MySQL
```bash
mysql -u root --password='re:St@rt!9'

```

### 🔹 Criar Banco de Dados
```bash
CREATE DATABASE world;
SHOW DATABASES;

```

### 🔹 Criar Tabela
```bash
CREATE TABLE world.country (
  Code CHAR(3) NOT NULL,
  Name CHAR(52) NOT NULL,
  Continent ENUM('Asia','Europe','North America','Africa','Oceania','Antarctica','South America') NOT NULL,
  Region CHAR(26) NOT NULL,
  Population INT NOT NULL,
  PRIMARY KEY (Code)
);

```

### 🔹 Listar Tabelas e Colunas
```bash
USE world;
SHOW TABLES;
SHOW COLUMNS FROM world.country;

```

### 🔹 Alterar Estrutura da Tabela
```bash
ALTER TABLE world.country RENAME COLUMN Continent TO Continente;


```

### 🔹 Criar Nova Tabela (Exemplo)
```bash
CREATE TABLE world.city (
  Name CHAR(52),
  Region CHAR(26)
);

```

### 🔹 Excluir Tabela
```bash
DROP TABLE world.city;
DROP TABLE world.country;

```

🔹 Excluir Banco de Dados
```bash
DROP DATABASE world;
SHOW DATABASES;

```

✅ Conclusão
Com este guia você pode:

Criar bancos e tabelas(CREATE)

Consultar bancos e tabelas(SHOW)

Alterar estruturas(ALTER)

Excluir tabelas e bancos(DROP)


---

