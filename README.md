# BRD_Cifras

Site de cifras musicais (letra + acordes), desenvolvido para fins educacionais.

## Stack

- **Backend:** Java + Spring Boot (API REST)
- **Frontend:** JavaScript puro (Vite, sem framework)
- **Banco de dados:** PostgreSQL, hospedado no Supabase (futuramente pode migrar para uma instância PostgreSQL própria — Supabase já é PostgreSQL por baixo dos panos, então a migração é só de host/conexão)

## Status do projeto

🚧 Em planejamento/desenvolvimento inicial. Ainda não há código de backend ou frontend implementado — o projeto está na fase de modelagem.

Planejamento completo em [`docs/Site de Cifras - Planejamento.txt`](docs/Site%20de%20Cifras%20-%20Planejamento.txt).

## Funcionalidades

### V1 (em andamento)
- Listar músicas cadastradas
- Visualizar a cifra de uma música (letra + acordes)
- Buscar música por nome/artista

### Futuras melhorias
- Transposição de tom
- Login e cadastro de usuário
- Favoritar músicas
- Comentários
- Upload de cifras por usuários

## Modelagem de dados

**Artista**
- nome
- descrição
- relacionamento: um artista possui várias músicas (1:N)

**Musica**
- título
- data de lançamento
- artista (referência ao Artista)
- corpo da cifra

O corpo da cifra segue o formato de acordes em uma linha separada, acima da letra:

```
C          G
Se você quer saber de mim
```

## Como rodar

Instruções de execução serão adicionadas assim que o backend e o frontend estiverem implementados.
