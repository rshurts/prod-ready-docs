# Production Ready Documentation


### What is Production Ready Documentation?

Production ready documentation is documentation that can be trusted to support a product running production traffic. This means the documentation is complete, up-to-date, and readily available. The documentation includes all the relevant and essential information necessary to understand the product.

Good documentation increases developer productivity, helps resolve issues faster, and creates a shared understanding of the product. This is because product ready documentation adopts a "self-service" mindset, where the documentation provides all the information for a person to solve their own problems just by reading the documentation.

While we seek to write maintainable, easy to read code, "there is no such thing as self-documenting code. While well-written code can tell you _what_ it does, no programming language ... can tell you _why_ it does it. This is why all software needs documentation beyond the code itself." (Brikman, _Terraform Up & Running: Writing Infrastructure as Code_, p. 154-155)

> **Comments Are Not Documentation**
>
> While comments are an essential piece of well written code, they are not production ready documentation. We don't want people to have to checkout and search through code to understand the product.


### Creating Production Ready Documentation

To assist in creation of production ready documentation, this [Gitbook](https://www.gitbook.com/) was created as a self service tool. To get started, follow these steps:

1. Install the gitbook-cli.
```
npm install --global gitbook-cli
```

1. Clone the prod-ready-docs git repository.
```
git clone git@github.com:rshurts/prod-ready-docs.git
```

1. Copy `/docs` and `book.json` from the cloned repository to the top level directory of your project. To keep your existing `README.md` as the introduction, instead of writing a new one, link it to `docs/README.md`.
```
ln -s README.md docs/README.md
```

1. Run `gitbook serve` and open [`localhost:4000`](http://localhost:4000) to see live edits of the documentation.

1. Read each page's description and update the markdown file to document your project.

1. Update the table of contents in the `SUMMARY.md` or add pages as needed.

1. Run `gitbook serve` to build the static site to host or distribute. Or generate a PDF or eBook by following [these instructions](https://toolchain.gitbook.com/ebook.html).

> **Include Documentation in Version Control**
>
> By including the /docs in the project, the documentation is now in version control. Because the documentation is plain text and lives with the source code, this allows documentation to be updated in parallel to code changes, easily `diff`ed, and results in the documention being versioned and tagged with the source code.
