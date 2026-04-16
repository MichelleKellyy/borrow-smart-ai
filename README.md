# borrow-smart-ai
Building this because I always want to read a book right away and also like getting AI to tell me which i'm gonna like, which gets to be a hassle as a picky reader

## API & Data Source

This project uses OverDrive's internal Thunder API (thunder-api.overdrive.com), the same backend that powers the Libby app. It is undocumented, unofficial, and requires no authentication.

This is a personal project, not affiliated with or endorsed by OverDrive. It is not intended for production use. OverDrive may restrict access at any time. For production apps, use the official API at [developer.overdrive.com](https://developer.overdrive.com/).

### Endpoints used
GET /v2/libraries/{libraryKey} — *library lookup*

GET /v2/libraries/{libraryKey}/media — *title search*

GET /v2/libraries/{libraryKey}/media/{titleId}/availability — *availability*

POST /v2/libraries/{libraryKey}/media/availability — *bulk availability*

GET /v2/libraries/{libraryKey}/media/{titleId}/recommended — *recommendations*
