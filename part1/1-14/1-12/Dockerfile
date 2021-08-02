# pull node, expose port 5000, set working directory
FROM node:14
EXPOSE 5000
WORKDIR /usr/src/app

# copy project files, install dependencies
COPY . .
RUN npm install
RUN REACT_APP_BACKEND_URL=http://localhost:8080 npm run build

# to serve static files
RUN npm install -g serve
CMD serve -s -l 5000 build