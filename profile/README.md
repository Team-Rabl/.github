# Enter: Rabl

Currently planned features:
- E2EE
- Direct Messaging
- Group Messaging

Current technologies used and or in consideration for use

# Backend
* PostgreSQL: Currently in use for auth server. Currently planning to use for application server. Exploring a NoSQL database may be worth the effort in the future.
* Actix (Rust): Currently in use for auth server. Webserver framework. Currently planning to use for application server as well.

# Frontend
* React: Has been discussed, and seems to be the current planned implementation for Desktop application via Electron, likely web version as well if a web version is desired to be released. Dioxus is a "React like" Rust frontend framework that would give lower level control, allowing for more targeted desktop development. Seems like potentially a good option, but needs research.
* NextJS: Being investigated for use in desktop app development.
* SCSS: Has been mentioned as being familiar to some of us, simple to learn/use.
Tailwind: Maybe? As a better alternative to Bootstrap? (If we need it? Hand made SCSS may be enough?)
* Flutter (Dart): Planned to be used for mobile application development.
