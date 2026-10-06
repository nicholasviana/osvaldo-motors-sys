[Atividade_05-Modelagem_BD_Clientes.md](https://github.com/user-attachments/files/33120540/Atividade_05-Modelagem_BD_Clientes.md)
# 🗄️ Atividade 05 - Modelagem de Banco de Dados (MER e DER)

## 🎯 Objetivo da Atividade
*(Capacidades: Modelar banco de dados relacionais / Aplicar normalização)*
Transformar os requisitos extraídos na entrevista com os 4 Clientes IA em modelos visuais de Banco de Dados (MER e DER) para que os sistemas possam armazenar informações reais.

---

## 📝 Contexto

O Deploy dos 4 sites já está na Nuvem (Vercel)! Mas eles ainda são apenas "cascas" vazias de HTML. Para que a Oficina do Seu Osvaldo consiga salvar um carro, ou a Dona Neide consiga receber uma encomenda de bolo, precisamos de um **Banco de Dados**.

Na engenharia de software, nós não abrimos o PostgreSQL e começamos a criar tabelas "da nossa cabeça". Se fizermos isso, as tabelas não vão se conectar direito, gerando inconsistência de dados. Primeiro, nós desenhamos a arquitetura do banco visualmente.

---

## 📋 Passo a Passo (Como Executar)

Você deverá realizar a modelagem para **os 4 clientes** da sua carteira. 

### Passo 1: O MER (Modelo Entidade-Relacionamento)
Para cada cliente, releia as anotações da sua entrevista (Atividade 02) e identifique:
1. **Entidades:** Quais são as "coisas" que precisam ser salvas? (Ex: Cliente, Produto, Consulta).
2. **Atributos:** Quais dados cada entidade tem? (Ex: Nome, CPF, Preço, Cor).
3. **Relacionamentos:** Como elas se conectam? (Ex: 1 Paciente agenda N Consultas).
*Você pode escrever o MER em formato de texto no próprio README.md de cada repositório.*

### Passo 2: O DER (Diagrama Entidade-Relacionamento)
Agora, vamos transformar o texto em desenho técnico!
1. Acesse o **brModelo**, **Figma**, **Draw.io** ou **Lucidchart**
2. Para cada cliente, desenhe as tabelas, identificando:
   - **PK (Primary Key):** A chave primária (ID).
   - **FK (Foreign Key):** A chave estrangeira que conecta as tabelas.
   - Os tipos de dados (INT, VARCHAR, BOOLEAN, DATE).
3. Exporte o desenho como imagem (PNG/JPG).

### Passo 3: Commit no Repositório
1. Pegue a imagem do DER da Dona Neide e salve na pasta do repositório dela. Pegue a do Seu Osvaldo e salve na dele, e assim por diante.
2. Atualize o `README.md` de cada projeto para exibir essa imagem (`![Diagrama DER](./der.png)`).
3. Faça o `git add .`, `git commit -m "docs: adiciona diagrama DER"` e `git push`.

---

## 🚀 Entregável
- Os repositórios do GitHub dos **4 clientes** atualizados com as imagens dos respectivos DERs aparentes no README.

---

## 📊 Rúbrica de Avaliação

| Critério | Atende Plenamente (3 pts) | Atende Parcialmente (1.5 pts) | Não Atende (0 pts) |
| :--- | :--- | :--- | :--- |
| **Integridade Relacional** | Os 4 diagramas possuem PKs, FKs corretas e conectam as entidades com as cardinalidades certas (1:N, N:M). | Fez o diagrama, mas esqueceu as Chaves Estrangeiras (FK) ou usou tipos de dados errados. | Não entregou os diagramas ou fez tabelas totalmente soltas e sem sentido. |
| **Aderência aos Requisitos** | O banco de dados reflete exatamente as regras de negócio de cada IA (ex: paciente VIP, taxa de urgência). | Modelou o banco, mas esqueceu de incluir atributos importantes pedidos pela IA na entrevista. | Entregou um modelo genérico que não atende as 4 IAs. |
