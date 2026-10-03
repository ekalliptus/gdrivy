# gdrivy

Web app to download files from Google Drive. React frontend with an Express server that proxies the Google Drive API.

## Features

- Download Google Drive files through a Drive API proxy
- Download progress via the X-Download-Progress header
- Works with Google OAuth credentials or an API key

## Tech Stack

- Frontend: React 18, Vite, Zustand, Axios
- Server: Express, googleapis, express-session
- Tests: Vitest on both frontend and server

## Getting Started

The server reads Google credentials from environment variables: `GOOGLE_API_KEY`, `GOOGLE_CLIENT_ID`, `GOOGLE_CLIENT_SECRET`, `GOOGLE_REDIRECT_URI`, `SESSION_SECRET`.

```sh
npm install
npm run dev:all
```

`dev:all` starts the Vite dev server and the API server together.

Build:

```sh
npm run build:all
```

Run tests:

```sh
npm run test:all
```

## License

MIT. See [LICENSE](LICENSE).
