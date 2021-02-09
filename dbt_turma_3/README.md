# Bootcamp Engenharia de Dados - DBT

###  Instalando DBT
```
pip install dbt
```


### Criando perfil
Crie um arquivo `~/.dbt/profiles.yml` com o seguinte conteúdo:
   ```yaml
   redshift:
      target: dev
      outputs:
        dev:
          type: redshift
          threads: 2
          host: seu-host-redshift
          port: 5439
          user: seu-usuario
          pass: sua-senha
          dbname: nome-do-db
          schema: dbt_dev_bootcamp
   ```

### Executando o projeto

Acesse a pasta da turma e tente executar:
- dbt run
- dbt test


### Resources:
- Learn more about dbt [in the docs](https://docs.getdbt.com/docs/introduction)
- Check out [Discourse](https://discourse.getdbt.com/) for commonly asked questions and answers
- Join the [chat](http://slack.getdbt.com/) on Slack for live discussions and support
- Find [dbt events](https://events.getdbt.com) near you
- Check out [the blog](https://blog.getdbt.com/) for the latest news on dbt's development and best practices
