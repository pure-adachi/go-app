# tips

## Go Lang Install

```sh
$ brew install go
```

### ルートを設定する為に gorilla/mux を使用するのでインストール

```sh
$ go get -u github.com/gorilla/mux
```

### Golang 用 ORM ライブラリインストール

```sh
$ go get -u github.com/jinzhu/gorm
```

### PostgreSQL

```sh
$ go get github.com/lib/pq
```

### Create Database Table Role

```
postgres=# create database "go-test";
go-test=# create table books (id INTEGER NOT NULL, title CHAR(255) NOT NULL, PRIMARY KEY (id));
go-test=# CREATE ROLE postgres;
go-test=# ALTER ROLE "postgres" WITH Superuser;
go-test=# ALTER ROLE "postgres" WITH LOGIN;
go-test=# INSERT INTO books(id, title) VALUES(1, 'book1');
```
