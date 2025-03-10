# Volume Directories

This directory contains persistent data for the Docker containers:

- **postgres/**: PostgreSQL database files
- **pictrs/**: Image storage for Pictrs (Picture/media service)

These directories will be populated when the Docker containers are started.

## Important Note

When transferring this repository to another machine, you might need to:

1. Create these directories manually if they don't exist:
   ```bash
   mkdir -p postgres pictrs
   ```

2. Set appropriate permissions:
   ```bash
   chmod 777 postgres pictrs
   ```

This ensures the Docker containers can write to these directories.