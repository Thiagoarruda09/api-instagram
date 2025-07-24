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

```mermaid
classDiagram 
    Usuario --> post: OneTomany    
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

    }
    class curtida{

    }
    ```
