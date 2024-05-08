FROM quay.io/shefin/alexa:md
RUN git clone https://github.com/shefin-xyz/whatsapp-bot-md.git /root/LyFE/
WORKDIR /root/LyFE/
RUN yarn install --network-concurrency 1
CMD ["npm", "start"]
