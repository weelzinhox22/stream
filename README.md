# WelPlayTV

A React application for loading and playing M3U playlists from remote URLs. This app features:

- Backend proxy server to handle CORS restrictions when loading remote M3U playlists
- User-friendly interface to browse and play content from M3U playlists
- Categories for Movies, Series, and TV Channels
- Video player with resume functionality and skip intro option
- Progress tracking for watched content

## Setup

1. Clone the repository
2. Install dependencies for both server and client:
   ```
   npm run install-all
   ```

## Running the App

Start both the backend and frontend with a single command:

```
npm start
```

This will start:
- The Express server on port 5000
- The React client on port 3000

## How to Use

1. Open the app in your browser (http://localhost:3000)
2. Enter an M3U playlist URL in the input field (e.g., https://is.gd/angeexx)
3. Click "Load Playlist" to fetch and parse the playlist
4. Browse through the categories and click on any item to play it
5. The app will remember your last-watched position for each video

## Building for Production

To build the client for production:

```
npm run build
```

The production build will be created in the `client/build` directory. The Express server is configured to serve these files in production mode.

## Technologies Used

- React for the frontend UI
- Express.js for the backend server
- Styled Components for styling
- Framer Motion for animations
- React Player for video playback
- Axios for HTTP requests

## License

ISC 