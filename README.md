
# hiring-lab/pages

## Requirements

- GitHub account with write access to the `hiring-lab/pages` repository.

## Add a New Interactive Plot Workflow

1) Add the `.html` and any required supporting files to the repo, organized in a subdirectory that describes the project (e.g. `job-transitions-sankey-diagrams`). Use lowercase, hyphen-separated names for directories and files.

2) Commit and push your changes to the `main` branch.

3) Navigate to https://github.com/hiring-lab/pages/settings/pages

4) Under the 'Branch' heading, switch the source from `main` to `None`. 

5) Refresh the page, then set the source back to `main`. (This is required to force GitHub Pages to re-trigger a deployment.)

6) Deployments can be monitored here: https://github.com/hiring-lab/pages/actions/workflows/pages/pages-build-deployment

## Hosted Plot URLs

The base URL for hosted plots is https://hiring-lab.github.io/pages/

As an example, the file located at `pages/job-transitions-sankey-diagrams/UK-dropdown-interactive-sankeys.html` will have the following URL:
https://hiring-lab.github.io/pages/job-transitions-sankey-diagrams/UK-dropdown-interactive-sankeys.html

Other `.html` files follow the same pattern of appending the file path to the base URL.

## Considerations

GitHub Pages does not offer server-side rendering; hosted content is rendered entirely by the browser. This means there are practical limits to how large your `.html` files can be without causing frustrating load times. As a rough guideline, aim to keep files under **10 MB**; anything larger will likely result in long load times for users with typical connections.

An interactive image width of **700 pixels** seems to work nicely with the WordPress Advanced iFrames used in Hiring Lab blog posts.
