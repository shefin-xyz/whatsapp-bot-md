FROM node:lts-buster

RUN git clone https://github.com/shefin-xyz/whatsapp-bot-md.git /root/LyFE/
WORKDIR /root/LyFE/

RUN apt-get update && \
  apt-get install -y \
  ffmpeg \
  imagemagick \
  webp && \
  apt-get upgrade -y && \
  rm -rf /var/lib/apt/lists/*

COPY package.json .

RUN npm install 

COPY . .

EXPOSE 3000

CMD ["npm", "start"]
