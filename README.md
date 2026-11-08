# MySQL on Linux Mint Lab
A hands-on learning project documenting MySQL setup and SQL practice on Linux Mint.


## Project Overview

This project documents my experience setting up and exploring MySQL on Linux Mint. I created this lab to practice managing a database server, importing a sample database, and writing SQL queries.

The project builds on concepts I am learning in my database coursework and provides a local environment where I can continue practicing.

## Objectives

- Verify that MySQL is installed and running.
- Connect to MySQL through the Linux terminal.
- Import the MySQL `world` sample database.
- Explore database tables and run SQL queries.
- Continue practicing database concepts and documenting my progress.

## Lab Environment

| Component | Details |
| --- | --- |
| Operating system | Linux Mint 22.3 Cinnamon |
| Database server | MySQL 8.0.46 |
| Interface | Linux terminal and MySQL command-line client |
| Sample database | MySQL `world` database |

## Project Status

**In progress:** MySQL is running, and I have imported and queried the `world` sample database. I plan to continue adding queries, examples, and documentation as I learn.

## Verify MySQL

I used the following commands to confirm that MySQL was installed and the server was running.

### Check the MySQL version

```bash
mysql --version
```

This displayed MySQL version **8.0.46** in my environment.

### Check the MySQL service

```bash
systemctl status mysql
```

The service status showed **active (running)** and **enabled**.

### Connect to MySQL

```bash
sudo mysql
```

This opened the MySQL command-line monitor.

### Verify the server version and list databases

At the `mysql>` prompt, I ran:

```sql
SELECT VERSION();
SHOW DATABASES;
```

The output displayed the server version and the default databases available at the time.

### Exit MySQL

```sql
EXIT;
```

This returned me to the Linux terminal.
