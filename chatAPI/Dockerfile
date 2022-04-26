FROM node

# Copy function code
WORKDIR /home/node/app

COPY *.js /home/node/app/
COPY package*.json /home/node/app/

RUN ["npm","install"]
ENV NODE_ENV=production

# Set the CMD to your handler (could also be done as a parameter override outside of the Dockerfile)
CMD [ "node","index.js" ]
EXPOSE 3000