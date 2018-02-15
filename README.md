# Lynx Framework
[![FOSSA Status](https://app.fossa.io/api/projects/git%2Bgithub.com%2Fmentos1386%2Flynx.svg?type=shield)](https://app.fossa.io/projects/git%2Bgithub.com%2Fmentos1386%2Flynx?ref=badge_shield)


## Built with

- [Nest.js](http://nestjs.com/) for Angular-like structure and dependency injection
- [TypeORM](http://typeorm.io/) for ORM with database
- [class-validator](https://github.com/pleerock/class-validator) for input validation

## Usage

### Install
```
$ npm install
```
Create new file `.env` in project root folder using `example.env` as a template. 

### Start

Development environment:
```
$ npm run start
```

Production environment:
```
$ npm run prestart:prod
$ node dist/src/api.ts
```

### Initial database creation
```
$ npm run migrate sync
```

### Migrations
Creating new migration named `createSomeModel`:
```
$ npm run migrate create createSomeModel
```
Other commands are self-explanatory:
```
$ npm run migrate [up|down|executed|pending|create]
```

### E2E Testing
First run the testing server:
```
$ npm run start:test
```
Then run Mocha testing framework:
```
$ mocha test/*.spec.ts
```
Before hooks in `test/` directory will clean test database, initialize sequelize and seed fake data. 


## License
[![FOSSA Status](https://app.fossa.io/api/projects/git%2Bgithub.com%2Fmentos1386%2Flynx.svg?type=large)](https://app.fossa.io/projects/git%2Bgithub.com%2Fmentos1386%2Flynx?ref=badge_large)