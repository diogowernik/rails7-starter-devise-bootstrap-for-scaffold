## How to use

### clone from github

    git clone https://github.com/diogowernik/rails7-starter-devise-bootstrap-for-scaffold.git your_app
    cd your_app

Change the name of database at `config/database.yml`

```

default: &default
adapter: postgresql
encoding: unicode
pool: <%= ENV.fetch("RAILS_MAX_THREADS") { 5 } %>

development:
<<: \*default
database: your_app_development

test:
<<: \*default
database: your_app_test

production:
<<: \*default
database: your_app_production
username: your_app
password: <%= ENV["RAILS_FINANCE_DATABASE_PASSWORD"] %>

```

Run the commands:

    bundle install
    rails db:create && rails db:migrate
    yarn
    bin/dev

Bugs known:

    - Login Page doesn`t validation errors

```

```
