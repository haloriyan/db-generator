# DB Generator
This is just simple way to generate/create a mysql database (like migration at Laravel)

# Installation
```
git clone https://github.com/haloriyan/db-generator.git
```

# How to use?
- First, star this repo, after that clone it
- After cloning, open the `db.json` file
- You can create or change database and table according to your needs in this file
- Run `create.php` with your browser

# Documentation

## Database name
```
{
  "namaDb": "myDb"
  ...
}
```
I think there's no difficulty here

## Setting up the tables
```
{
  ...
  "tabel": {
    "table1": [
      "id int(11)",
      "name varchar(20)",
      "dummy varchar(10) null"
    ],
    "table2":
    "table3":
    "etc"
  }
}
```
`id`, `name`, and `dummy` are names of your structures table. `int` and `varchar` are datatype of the structure. And `null` is optional. If you dont type it, that mean set to default which mean `not null`.

## Giving extra attribute
You can give extra attribute like primary key or unique key to your table structure like this
```
{
  "tabel": {
    "table1" : [ ... ]
  },
  "atribut": {
    "primary key": [
      "table1.id",
      "table2.username"
      "table3.etc"
    ],
    "unique key": [
      "table1.name",
      "table2.email",
      "table3.etc"
    ]
  }
}
```
I think you already understand with this. `table1.id` in `primary key` is structure where is set up to be primary. So also with the unique key. `table1` is name of your table, and `id` is structur name of your table.
