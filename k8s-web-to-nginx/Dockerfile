FROM node:alpine

WORKDIR /app

# Install dependencies
COPY package.json package-lock.json ./

# Debugging step: list files to ensure the package.json is correctly copied
RUN ls -la /app

RUN npm install

# Copy the rest of the application code
COPY . ./

# Expose the application port
EXPOSE 3000

# Start the application
CMD ["npm", "start"]
