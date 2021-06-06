# Create a node project...
FROM node

# ...in this directory in Docker.
WORKDIR /client

# Then, copy the package.json file over...
COPY package.json /client/

# ...and run `npm install`.
RUN npm install

# Finally, copy the contents of the root to the client dir...
COPY . /client/

# ...expose the port 3000...
EXPOSE 3000

# ...and run `npm start`.
CMD [ "npm", "start" ]
