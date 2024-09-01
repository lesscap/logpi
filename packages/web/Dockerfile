FROM node:20-alpine

RUN node -v
RUN npm install -g pnpm

ENV TZ=Asia/Shanghai

WORKDIR /app

COPY . .

RUN pnpm install
RUN pnpm run build

EXPOSE 3000
CMD ["npm", "start"]
