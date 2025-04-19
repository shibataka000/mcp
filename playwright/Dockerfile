FROM node:22-slim
RUN npx -y playwright@1.51.1 install --with-deps
RUN adduser pwuser
USER pwuser
ENTRYPOINT ["npx"]
CMD ["-y", "@playwright/mcp@v0.0.9", "--headless"]
