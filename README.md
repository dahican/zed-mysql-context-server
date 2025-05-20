# Zed MySQL Context Server

This extension provides a Model Context Server for MySQL, for use with the Zed AI assistant.

It adds a `/mysql-schema` slash command to the Assistant Panel.

## Configuration

To use the extension, you will need to point the context server at a MySQL database by setting the `database_url` in your Zed `settings.json`:

```json
{
  "context_servers": {
    "mysql-context-server": {
      "settings": {
        "database_url": "mysql://myuser:mypassword@localhost:3306/mydatabase"
      }
    }
  }
}
```

## Usage

- `/mysql-schema <table-name>`: Retrieve the schema for the table with the given name.
- `/mysql-schema all-tables`: Retrieve the schemas for all tables in the database.
