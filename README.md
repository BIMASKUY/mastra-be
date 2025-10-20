# Simple Express + Supabase Backend

A simple Express.js backend that fetches data from Supabase tables.

## Setup

1. Install dependencies:
```bash
npm install
```

2. Create a `.env` file in the root directory:
```env
SUPABASE_URL=your_supabase_url_here
SUPABASE_ANON_KEY=your_supabase_anon_key_here
PORT=3000
```

3. Replace the placeholder values with your actual Supabase credentials.

## Run

```bash
npm start
```

Or for development with auto-reload:
```bash
npm run dev
```

## API Endpoints

- `GET /` - API info and available endpoints
- `GET /api/authors` - Fetch 4 authors
- `GET /api/books` - Fetch 4 books
- `GET /api/comments` - Fetch 4 comments
- `GET /api/reviews` - Fetch 4 reviews

## Response Format

All endpoints return JSON in this format:

```json
{
  "success": true,
  "count": 4,
  "data": [...]
}
```

On error:
```json
{
  "success": false,
  "error": "error message"
}
```
