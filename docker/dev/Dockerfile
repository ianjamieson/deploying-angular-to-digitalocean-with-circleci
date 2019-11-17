FROM circleci/node:12.13.0

#ENV NPM_CONFIG_PREFIX=/home/circleci/.npm-global

WORKDIR /home/circleci/app

COPY . .

RUN sudo npm install

EXPOSE 4200

CMD ./node_modules/@angular/cli/bin/ng serve --host 0.0.0.0 --port 4200
