# Stage 1: Build Stage
FROM node:alpine as builder

# Add maintainer label
LABEL maintainer="Pratik pratikgondkar4040@gmail.com"

# Update Alpine and install Node.js (it is preinstalled in the alpine version of node image)
RUN apk update && apk add --no-cache nodejs

# Set the working directory
WORKDIR /app

# Copy current directory to /app inside the container
COPY . .

# Install any dependencies (if you had package.json, you'd install dependencies here)
# RUN npm install

# Stage 2: Production Stage
FROM node:alpine

# Add maintainer label
LABEL maintainer="Pratik pratikgondkar4040@gmail.com"

# Copy only necessary files from the builder stage
COPY --from=builder /app /app

# Set the working directory to /app
WORKDIR /app

# Specify the default command to run
CMD ["node", "index.js"]
