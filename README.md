[![Cargo](https://img.shields.io/crates/v/slack_morphism.svg)](https://crates.io/crates/slack_morphism)
![tests and formatting](https://github.com/abdolence/slack-morphism-rust/workflows/tests%20&amp;%20formatting/badge.svg)
![security audit](https://github.com/abdolence/slack-morphism-rust/workflows/security%20audit/badge.svg)

# Slack Morphism for Rust

Slack Morphism is a modern client library for Slack Web/Events API/Socket Mode and Block Kit.

## Documentation
Please follow to the official website: https://slack-rust.abdolence.dev.

## Examples

https://github.com/abdolence/slack-morphism-rust/tree/master/src/hyper/examples

The examples require to work the following environment variables (from your Slack bot profile in api.slack.com):

- `SLACK_TEST_TOKEN` - for Slack client example
- `SLACK_TEST_APP_TOKEN` - for Slack client with Socket Mode example
- `SLACK_CLIENT_ID`, `SLACK_CLIENT_SECRET`, `SLACK_BOT_SCOPE`, `SLACK_REDIRECT_HOST` - for OAuth routes for Events API example
- `SLACK_SIGNING_SECRET` for all routes for Events API example

To run example use with environment variables:
```
# SLACK_... cargo run --example <client|events_api_server|socket_mode>
```

Routes for this example are available on http://<your-host>:8080:

- /auth/install - to begin OAuth installation
- /auth/callback - a callback endpoint for Slack OAuth profile config
- /push - for Slack Push Events
- /interaction - for Slack Interaction Events
- /command - for Slack Command Events

## Licence
Apache Software License (ASL)

## Author
Abdulla Abdurakhmanov
