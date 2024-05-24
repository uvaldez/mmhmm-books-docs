---
sidebar_position: 1
---

# Getting Started

Let's discover **mmhmm Bookshelf App**.

## Stack

* [NextJS 14](https://nextjs.org/)
* [ReactJS](https://react.dev/)
* [Tailwind CSS](https://tailwindcss.com/)
* [Docusaurus](https://docusaurus.io/)
* [Json-server](https://www.npmjs.com/package/json-server)
* [Typescript](https://www.typescriptlang.org/)

## Repositories
* [Application](https://github.com/uvaldez/mmhmm-books-uvaldez)
* [Documentation](https://github.com/uvaldez/mmhmm-books-docs)

## Running APP on the cloud
:::info
When running on the cloud the app depends on the [API](https://us-central1-all-turtles-interview.cloudfunctions.net) provided by the team at **mmhmm** if the API is down please try to run the project locally and follow instructions for mocking the data.
:::

To run the app on the cloud you just visit the following url: [mmhmm-books-app](https://mmhmm-books-uvaldez.onrender.com)

## Running the APP local

### What you'll need

- [Node.js](https://nodejs.org/en/download/) version 18.0 or above:
  - When installing Node.js, you are recommended to check all checkboxes related to dependencies.

**Clone the APP**

Clone frontend [app repo](https://github.com/uvaldez/mmhmm-books-uvaldez) from github, use the following command:

```bash
git clone https://github.com/uvaldez/mmhmm-books-uvaldez.git mmhmm-books-uvaldez
```

Move to directory
```bash
cd mmhmm-books-uvaldez
```

Install dependencies
```bash
npm install
```

Run project
```bash
npm run dev
```

APP should be running on http://localhost:3000/

**Test with mock data**

1. By default the app will be making requests to the [cloud endpoint](https://us-central1-all-turtles-interview.cloudfunctions.net) to change the base url navigate to `src/data/constants.js` file and replace `SERVICE_BASE_URL` with local API url http://localhost:4000/
2. Open a new terminal tab and cd to `mmhmm-books-uvaldez`
3. Run `json-server --watch --port 4000 ./src/data/db.json` this will create a new server at port `4000` and serve the data from `./src/data/db.json` (<b>note:</b> this will only work for listing or viewing books not for creating new books)
