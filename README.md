# [@superfast_news_bot](https://t.me/superfast_news_bot)

## Overview
Telegram bot that monitors multiple Telegram channels and provides AI-powered consolidated news digests by identifying and grouping duplicate or similar stories across channels.

## Core Capabilities

### Channel Management
- **Subscribe to channels** (`/add @channel`) - Monitor up to 10 public Telegram channels
- **Unsubscribe** (`/remove @channel`) - Remove individual channels from monitoring
- **Bulk removal** (`/remove_all`) - Clear all subscribed channels at once
- **View subscriptions** (`/list`) - Display all currently monitored channels

### News Aggregation
- **AI-powered news digest** (`/news`) - Generate consolidated news summary with:
  - Automatic detection of duplicate/similar stories across channels
  - Source attribution showing which channels covered each story
  - Coverage count indicating story popularity

### Customization Options
- **Time range control** (`/time [hours]`) - Configure news lookback period:
  - Default: 24 hours
  - Range: 1-720 hours (30 days)
- **Summary limit** (`/posts [count]`) - Set maximum number of news summaries:
  - Default: 10 summaries
  - Range: 1-30 summaries

### Rate Limiting
- 5 news digest requests per user per day
- Automatic daily reset

## Commands Reference

- `/start` - Welcome message and introduction
- `/help` - Display available commands
- `/add @channel` - Subscribe to a channel
- `/remove @channel` - Unsubscribe from a channel
- `/remove_all` - Remove all channels
- `/list` - Show subscribed channels
- `/time [hours]` - View/set news time range
- `/posts [count]` - View/set max summaries
- `/news` - Generate news digest
