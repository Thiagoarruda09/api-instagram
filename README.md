# api-instagram

## tecnologias 
- node
- expressJS
- MySQL

### recursos 
- usuarios
- posts
- comentarios
- curtidas 

### estrutura de dados 

```classDiagram 
    Usuario --> post: OneTomany 
    Usuario --> comentario: OneTomany 
    post --> comentario: OneTomany 
    post --> curtida:OneTomany
    Usuario --> curtida:OneTomany
     
    class Usuario {
        + id
        + nome
        + nickname
        + bio
        + foto
        + email
        + senha
        + criado_em
        + atualizado_em

    }
    class post{
        + id 
        + usuario_id
        + foto
        + legenda?
        + Localizacao?
        + criado_em
        + atualizado_em?
        }
    class comentario{
        + id
        + usuario_id
        + post_id
        + conteudo
        + criado_em

    }
    class curtida{
        + id
        + usuario_id
        + post_id
        + criado_em

    }
    ```
