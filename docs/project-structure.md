---
sidebar_position: 3
---

# Project Structure

### api
All API requests and related should live in this folder.
- `books.ts` contains all API request related to bookshelf app.
  * Relative Path: `src/api/books.ts`
  * Repository Path: https://github.com/uvaldez/mmhmm-books-uvaldez/blob/main/src/api/books.ts
- `booksApi.ts` this is a wrapper for making API calls, it uses the facade design patter.
  * Relative Path: `src/api/booksApi.ts`
  * Repository Path: https://github.com/uvaldez/mmhmm-books-uvaldez/blob/main/src/api/booksApi.ts


### app
All routes pages should live here.
* `add` folder contains the add page where adding a form action lives.
  * Relative Path: `src/app/add/page.tsx`
  * Repository Path: https://github.com/uvaldez/mmhmm-books-uvaldez/blob/main/src/app/add/page.tsx
* `book[id]` folder contains the single view for a book.
  * Relative Path: `src/app/book/[id]/`
  * Repository Path: https://github.com/uvaldez/mmhmm-books-uvaldez/tree/main/src/app/book/%5Bid%5D
* `page.tsx` this is the home page.
  * Relative Path: `src/app/page.tsx`
  * Repository Path: https://github.com/uvaldez/mmhmm-books-uvaldez/blob/main/src/app/page.tsx

### assets
This folder should handle all assets like css files and images.

### components
The components folder should handle all generic components that are shared across the application, if there are components for specific feature, they should live in it's onw folder, example `https://github.com/uvaldez/mmhmm-books-uvaldez/tree/main/src/components/features/bookshelf`

### data
This folder has two files for now but everything related to data should live here.
* `constants.js` all constants.
  * Relative Path: `src/data/constants.ts`
  * Repository Path: https://github.com/uvaldez/mmhmm-books-uvaldez/blob/main/src/data/constants.ts
* `db.json` local database to mock data.
  * Relative Path: `src/data/db.json`
  * Repository Path: https://github.com/uvaldez/mmhmm-books-uvaldez/blob/main/src/data/db.json

### services
In this folder everything related to services should be added here, example interfaces, models, etc.
* `interfaces` all interfaces.
  * `book.ts` interface for books.
    * Relative Path: `src/services/interfaces/book.ts`
    * Repository Path: https://github.com/uvaldez/mmhmm-books-uvaldez/blob/main/src/services/interfaces/book.ts

## utils
All util files.
* `revalidateTag.ts` this clears cache after a new book is added.
  * Relative Path: `src/utils/revalidateTag.ts`
  * Repository Path: https://github.com/uvaldez/mmhmm-books-uvaldez/blob/main/src/utils/revalidateTag.ts
