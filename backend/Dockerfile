# Step 1: Use an official Node.js image as a base image
FROM node:16

# Step 2: Set the working directory inside the container
WORKDIR /app

# Step 3: Copy package.json and package-lock.json from the root directory to the container
COPY ../package*.json ./

# Step 4: Install the dependencies inside the container
RUN npm install

# Step 5: Copy the rest of the application code to the container
COPY . .

# Step 6: Expose the port the Node.js app will run on
EXPOSE 5000

# Step 7: Start the Node.js app when the container starts
CMD ["npm", "start"]
