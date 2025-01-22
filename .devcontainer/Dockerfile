# GitHub Codespaces development container for Spring Boot + Vue.js + PostgreSQL
FROM mcr.microsoft.com/devcontainers/java:20

# Install Node.js, npm, and Vue CLI
RUN apt-get update && \
    apt-get install -y curl gnupg && \
    curl -fsSL https://deb.nodesource.com/setup_16.x | bash - && \
    apt-get install -y nodejs && \
    npm install -g @vue/cli

# Install PostgreSQL client
RUN apt-get install -y postgresql-client

# Set up working directory
WORKDIR /workspace
