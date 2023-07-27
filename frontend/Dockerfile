
FROM node:14
WORKDIR /app
COPY package.json package-lock.json ./
RUN npm install
COPY . .

# RUN sed -i 's/localhost:5000/<name of cluster ip>/g' *
# This line runs a find command to locate all the files (-type f) within the /app directory and then uses sed to replace occurrences of http://localhost:5000 with https://dhanush.com in those files. 
# This is likely another way to update the API endpoint URLs in the React application for deployment
RUN find /app -type f -exec sed -i 's/http:\/\/localhost:5000/https:\/\/shwetha.com/g' {} +
#localhost:5000
CMD ["npm", "start"]
