# Enter: Rabl

Currently planned features:
- E2EE
- Direct Messaging
- Group Messaging

Current technologies used and or in consideration for use

* Backend
PostgreSQL: Currently in use for auth server. Currently planning to use for application server. Exploring a NoSQL database may be worth the effort in the future.
Actix (Rust): Currently in use for auth server. Webserver framework. Currently planning to use for application server as well.

* Frontend
React: Has been discussed, and seems to be the current planned implementation for Desktop application via Electron, likely web version as well if a web version is desired to be released. Dioxus is a "React like" Rust frontend framework that would give lower level control, allowing for more targeted desktop development. Seems like potentially a good option, but needs research.
SCSS: Has been mentioned as being familiar to some of us, simple to learn/use.
Tailwind: Maybe? As a better alternative to Bootstrap? (If we need it? Hand made SCSS may be enough?)
Flutter (Dart): Would be a great option for mobile application deployment. React Native would work for mobile, but Flutter seems to just be "better", and Tyler is our most experienced mobile dev, likely we should leave the mobile decisions to him

* Architecture
Github: Source control, planning, todos, issues
DigitalOcean: VPS Hosting? Alternative is AWS EC2 which seems to be cheap, but vendor lock-in creeps up very quickly with AWS
HAProxy: Reverse proxy software
Firewall: Idk. we need to determine a way to setup a firewall so that only us devs can connect directly to DB, build server, app servers, etc. Private VPNs are a common solution. IP address whitelists is as        well, but does not work if any of our IP addresses will change frequently.
Backups (Database): Probably just gzip and dump to an AWS S3 bucket. It's the simplest solution I can think of, and S3 is very cheap with something like first 500GB of free space.
