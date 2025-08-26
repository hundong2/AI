# Gemini

## local build install for gemini

- npm, npx install latest version

### nvm node package managing tool 

- [nvm-sh/nvm github](https://github.com/nvm-sh/nvm)
- [gemini](https://github.com/google-gemini/gemini-cli/blob/main/CONTRIBUTING.md) 

```sh
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.40.3/install.sh | bash
```

```sh
 curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.40.3/install.sh | bash
 source ~/.bashrc
 nvm -v
 nvm install node
 nvm install --lts
 nvm alias default lts/* #alias setting lts version, nvm alias default node 
 node -v
 npm -v
 npm install
 npm install -g npm@11.5.2 #2025.08.26 npm@11.5.2 need to gemini-cli
 npm -v
 npm install
 npm run build:all
 npm start #start gemini

```