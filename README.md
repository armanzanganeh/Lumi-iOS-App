# Lumi

**Lumi is an iOS app that helps people expand their cultural knowledge through daily tasks.**
It assigns small, engaging tasks across cinema, literature and music based on the user's interests, tracks progress, and shows cultural growth on an interactive world map.

Built for the **Federico II Apple Foundation Program** (Università degli Studi di Napoli Federico II – Apple Developer Academy), 2026.

## Idea

Infinite feeds and short-form content leave many people distracted and culturally isolated. Lumi turns everyday moments into opportunities for curiosity: instead of passive scrolling, users complete active tasks (watch a film, read a book, listen to an album) and build real cultural literacy step by step. Lumi is completely free, with no paywalls.

## Features

- **Personalized onboarding** based on the user's interests
- **Daily tasks** across films, books and music, with extra tasks the user can add
- **Interactive world map** (Mapbox): countries light up as tasks from them are completed
- **Browse and search** by category and by country
- **History and progress** with points and a congratulations screen when a task is completed
- **Rich details** for each work: poster or cover, story, rating, trailer link

## Tech stack

- Swift, SwiftUI (iOS 26+)
- Mapbox Maps SDK (Swift Package Manager)
- Data: [TMDB](https://www.themoviedb.org) (films), [iTunes Search](https://performance-partners.apple.com/search-api) and [MusicBrainz](https://musicbrainz.org) (music), [Open Library](https://openlibrary.org) (books), [Wikidata](https://www.wikidata.org) (countries of origin)
- Curated lists of award-winning and canonical works for films, books and music

## Getting started

1. Clone the repository and open `Lumi.xcodeproj` in Xcode 26 or later.
2. Open `Lumi-Info.plist` and replace the placeholders with your own keys:
   - `MBXAccessToken`: public token from [mapbox.com](https://www.mapbox.com) (needed for the world map)
   - `TMDBToken`: API key or read access token from [themoviedb.org](https://www.themoviedb.org/settings/api) (without it, films are still listed but without poster, story and rating)
3. In *Signing & Capabilities*, choose your own development team.
4. Build and run on a simulator or device.

> Never commit real keys. To keep your local keys out of Git, run:
> `git update-index --skip-worktree Lumi-Info.plist`

## Team: The Uniques

All members contributed across every part of the project: concept, design, development, content and presentation.

- Antonio Fornaro
- Arman Zanganeh
- Domenico Troiano
- Lorenzo Scognamiglio
- Rita Verrone
- Siria Scognamiglio
- Vittorio Ragosta
