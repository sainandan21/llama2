# Use a base image with the desired Linux distribution
FROM ubuntu:latest

# Install necessary dependencies
RUN apt-get update && apt-get install -y curl

# Download and install Ollama
RUN curl https://ollama.ai/install.sh | sh

# Download the Ollama binary
RUN curl -L https://ollama.ai/download/ollama-linux-amd64 -o /usr/bin/ollama
RUN chmod +x /usr/bin/ollama

# Start Ollama
CMD ["ollama", "serve"]
