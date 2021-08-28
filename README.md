instauto is an Instagram automation/bot library written in modern, clean
javascript using Google's Puppeteer. Goal is to be very easy to set up, use, and
extend, and obey instagram's limits.

## Setup

- First install [Node.js](https://nodejs.org/en/) 8 or newer.

- `headless: true` - you won't see what bot do
- `headless: false` - you will see what bot do
- `dryRun: true` - bot will work everything except liking and following
- `dryRun: false` - bot will work everything, include liking and following

## Create empty `database` directory so bot can generate json files where data will be stored

- Open a terminal in the directory

- Run `npm i -g yarn`

- Run `npm install puppeteer instauto dotenv`

- Run `node instaBot`

### You can run this code for example once every day using cron or pm2 or similar!!!

## Supported functionality

- Follow the followers of some particular users. (e.g. celebrities.) Parameters
  like max/min ratio for followers/following can be set.

- Unfollow users that don't follow us back. Will not unfollow any users that we
  recently followed.

- Unfollow auto followed users (also those following us back) after a certain
  number of days.

- The code automatically prevents breaching 100 follow/unfollows per hour or 700
  per 24hr, to prevent bans. This can be configured.
