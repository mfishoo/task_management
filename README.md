A NestJS API to manage tasks.

## Task Model
```
{
id: string,
title: string,
description: string,
status: enum(OPEN, DONE, IN_PROGRESS)
}
```

## End Points
- /tasks (@GET): get all tasks
- /tasks?status=xxx (@GET): search for tasks with status as xxx
- /tasks?search=xxx (@GET): search for tasks contain xxx in the title or description
- /tasks/:id (@GET): search a task by id
- /tasks (@POST)(@Body: title, description): create a task with title & description
- /tasks/:id (@DELETE): delete a task by id
- /tasks/:id/status (@PATCH)(@Body: status): update a task's status


## Installation

```bash
$ npm install
```

## Running the app

```bash
# development
$ npm run start

# watch mode
$ npm run start:dev

# production mode
$ npm run start:prod
```

