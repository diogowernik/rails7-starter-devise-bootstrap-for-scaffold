## create rails app

    rails new rails_finance -j esbuild --css bootstrap --database=postgresql --force

## install gems

    bundle add devise
    bundle add devise-i18n
    bundle add devise-bootstrap5

## create devise user

    rails generate devise:install
    rails generate devise User
    rails generate devise:views:bootstrap
    rails generate devise:i18n:views

## create home page

    rails generate controller Pages home

## migrations

    rails db:migrate

## creating custom scaffold
