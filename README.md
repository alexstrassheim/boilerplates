# Boilerplates
This is my personal template collection. Here you'll find templates, and configurations for various tools, and technologies.

## Boilerplate Information

In the provided boilerplates, the `stack-example.env` file uses the values `1000` for both **PUID** (User ID) and **GUID** (Group ID) by default.

These values are commonly used on many Linux systems, but they **may not match the user and group IDs on your environment**.

### Important
Before deploying or starting any stack, make sure to:

1. Check your local user ID and group ID.
2. Adjust the values in `stack-example.env` accordingly.
3. Ensure all mounted volumes and file permissions align with the chosen IDs.

Failing to update these values may result in:
- Permission errors
- Inaccessible mounted files
- Containers failing to start

To check your user and group ID on most Linux systems, run:

```bash
id
```
