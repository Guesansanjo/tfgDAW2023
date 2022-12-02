# Chapter 2 : Creacion proyecto.

---
Primeros pasos en Rails

---

```ruby
gem install rails
rails new <application_name> -d postgresql
bundle install
bundle update
```

Con estos comandos creamos un proyecto en Rails con DB Postgre.

Ejecutamos el sevidor ...

```ruby
rails s
```
![gem tzinfo-data error](/src/image/error1.png)

Este error se soluciona eliminando la gem o actualizandola.


```ruby
gem 'tzinfo-data', '~> 1.2022', '>= 1.2022.7'
```
Se modificara por esto en el Gemfile.

Configuramos la base de datos.

![Postgre](/src/image/configDB.png)

En database.yml en las tres instancias , development,test y production , ponemos nuestras credenciales.

- DB name
- Superuser
- Password
- Port

```ruby
rails s
```

Funciona correctamente , ya tenemos el esqueleto sobre el que montar nuestra webapp.

- [Summary ](./SUMMARY.md)