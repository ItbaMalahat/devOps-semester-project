# Step 1: Use an official Node.js image as the base image
FROM node:16

# Step 2: Set the working directory inside the container
WORKDIR /app

# Step 3: Copy package.json and package-lock.json to the container
COPY package*.json ./

# Step 4: Install the dependencies inside the container
RUN npm install

# Step 5: Copy the rest of the application code to the container
COPY . .

# Step 6: Expose the port the React app will run on
EXPOSE 3000

# Step 7: Start the React app when the container starts
CMD ["npm", "start"]
