# Installing on Linux
Vue Cloudfront is based on open source technologies which **should** in theory work perfectly well on most of the leading operating systems.
However, I develop the project using Windows machines.

## Requirements

1. Install [LTS version of Node.js for Mac](https://nodejs.org/en/download/)
2. Install [MongoDB for Mac](https://docs.mongodb.com/manual/tutorial/install-mongodb-on-os-x/)
3. You can [download Github Desktop](https://desktop.github.com/) to get access not only for fancy UI but for git toolset itself.

## Installation of vue-cloudfront-api

1. Open the terminal with [Git](https://git-scm.com/download/win) access or use Github desktop
2. Clone the [vue-cloudfront-api](https://github.com/Simonwep/vue-cloudfront-api) project:

```bash
git clone https://github.com/Simonwep/vue-cloudfront-api
```

3. Go to `vue-cloudfront-api` and install dependencies:

```bash
cd vue-cloudfront-api
npm install
```

4. Run vue-cloudfront-api:

```bash
npm run dev
```

## Installation of vue-cloudfront

1. Open your cmdline of choice with [Git](https://git-scm.com/download/win) access or use Github desktop
2. Clone the [vue-cloudfront](https://github.com/Simonwep/vue-cloudfront) project:

```bash
git clone https://github.com/DivanteLtd/vue-cloudfront.git
```

3. Go to `vue-cloudfront` directory and install dependencies:

```
cd vue-cloudfront
npm install
```

4. Configure `vue-cloudfront`  
Since nginx is not used during development there are two properties which need to be changed in [config.json](https://github.com/Simonwep/vue-cloudfront/blob/master/config/config.json):
```json
"apiEndPoint": "http://localhost:8080/api",
"websocketEndPoint": "ws://localhost:8080/ws"
```

5. Run Vue Cloudfront Server:

```bash
npm run dev
```

Now you should have Vue Cloudfront running on `localhost:3000`.
