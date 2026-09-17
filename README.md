# Backend Test Case

## Entities

- Member
- Book

## Use Case

- Members can borrow books with conditions
    - [ ]  Members may not borrow more than 2 books
    - [ ]  Borrowed books are not borrowed by other members
    - [ ]  Member is currently not being penalized
- Member returns the book with conditions
    - [ ]  The returned book is a book that the member has borrowed
    - [ ]  If the book is returned after more than 7 days, the member will be subject to a penalty. Member with penalty cannot able to borrow the book for 3 days
- Check the book
    - [ ]  Shows all existing books and quantities
    - [ ]  Books that are being borrowed are not counted
- Member check
    - [ ]  Shows all existing members
    - [ ]  The number of books being borrowed by each member

## Mock Data

- Books

```tsx
[
    {
        code: "JK-45",
        title: "Harry Potter",
        author: "J.K Rowling",
        stock: 1
    },
    {
        code: "SHR-1",
        title: "A Study in Scarlet",
        author: "Arthur Conan Doyle",
        stock: 1
    },
    {
        code: "TW-11",
        title: "Twilight",
        author: "Stephenie Meyer",
        stock: 1
    },
    {
        code: "HOB-83",
        title: "The Hobbit, or There and Back Again",
        author: "J.R.R. Tolkien",
        stock: 1
    },
    {
        code: "NRN-7",
        title: "The Lion, the Witch and the Wardrobe",
        author: "C.S. Lewis",
        stock: 1
    },
]
```

- Members

```tsx
[
    {
        code: "M001",
        name: "Angga",
    },
    {
        code: "M002",
        name: "Ferry",
    },
    {
        code: "M003",
        name: "Putri",
    },
]
```

## Requirements

- [ ]  Use TypeScript throughout the backend
- [ ]  Use [NestJS](https://nestjs.com/) as the framework
- [ ]  Use a SQL database via a modern ORM (e.g. Prisma, Drizzle, or TypeORM)
- [ ]  Use [pnpm](https://pnpm.io/) or [yarn](https://yarnpkg.com/) for dependency management and scripts
- [ ]  Document the REST API with [OpenAPI](https://www.openapis.org/) / Swagger
- [ ]  It should be open sourced on your github repo

## Extras

- [ ]  Implement [DDD Pattern]([https://khalilstemmler.com/articles/categories/domain-driven-design/](https://khalilstemmler.com/articles/categories/domain-driven-design/))
- [ ]  Implement Unit Testing
- [ ]  Provide a docker-compose setup for the API and database
- [ ]  Implement load testing with [k6](https://k6.io/)

## Notes
- Feel free to add some structure or plugins


# Frontend Test Case

- [ ] Create features based on the RESTful API that has been created using NestJS.
- [ ] It should use React
- [ ] It should use TypeScript
- [ ] It should use [Ant Design](https://ant.design/) for styling (you can customize the UI if you are interesting with UI/UX)
- [ ] Use [pnpm](https://pnpm.io/) or [yarn](https://yarnpkg.com/) for dependency management and scripts
- [ ] It should be open sourced on your github repo

## Extras
- [ ] Test your components with [jest](https://jest-everywhere.now.sh)
- [ ] It should use [Clean Architecture](https://medium.com/@rostislavdugin/the-clean-architecture-using-react-and-typescript-a832662af803) as design pattern
- [ ] Use a monorepo (e.g. pnpm/yarn workspaces) to host the API and web app together (plus point)
