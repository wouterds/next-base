FROM node:14-alpine
WORKDIR /code

COPY ./ ./

RUN yarn --frozen-lockfile
RUN yarn build

FROM node:14-alpine
WORKDIR /code

ENV NODE_ENV=production

CMD ["yarn", "start"]

COPY --from=0 /code/.next /code/.next
COPY ./public ./public
COPY ./package.json ./package.json
COPY ./yarn.lock ./yarn.lock

RUN yarn --production --frozen-lockfile
