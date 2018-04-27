# DB Generator
This is just simple way to generate/create a database (like migration at Laravel)

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
- Database name
```
{
  "namaDb": "myDb"
  ...
}
```
I think there's no difficulty here

- Setting up the tables
```
{
  ...
  "tabel": {
    "tabel1": [
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
