FROM debian:buster-slim AS dev

# Install texlive-full, git, and GitHub CLI
RUN apt-get update && \
    apt-get install --no-install-recommends -y texlive-full && \
    apt-get clean && \
    rm -rf /var/lib/apt/lists/*

# Verify installations
RUN xelatex --version

CMD ["xelatex", "--version"]