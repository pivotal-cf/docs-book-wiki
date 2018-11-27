Welcome to the Docs wiki.

## About this Repo
* This book repo is for building the master version of the internal Docs Wiki.
* The content repo is in pivotal-cf-experimental/docs-wiki-internal.
* The concourse pipeline that builds this book can be found under cf-current/docs-wiki

## How To Contribute

1. Navigate to [https://github.com/pivotal-cf-experimental/docs-wiki-internal](https://github.com/pivotal-cf-experimental/docs-wiki-internal).
1. Clone the `docs-wiki-internal` repo.
1. Make whatever changes you like.
1. Add, commit, and push your changes. 
1. To build a local copy of the Wiki, clone this Book repo for the Wiki (https://github.com/pivotal-cf/docs-book-wiki)
1. Watch your changes bind and stage in Concourse at
   [`cf-current/docs-wiki`](https://concourse.run.pivotal.io/teams/cf-docs/pipelines/cf-current?groups=docs-wiki).

## Automated Subnavs

The Docs Wiki uses automated subnavs.
So if you're adding a new topic, make sure to add it to the `index` of the section where it appears in the content repo.

For example, if you're adding a new topic called `foo.html.md.erb` to the `bookbinder` section,
make sure `index.html.md.erb` includes a link to the new topic with `class="subnav"`:

```
<a href="foo.html.md.erb" class="subnav">Foo</a>
