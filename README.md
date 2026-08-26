# docs

Documentation site for [Sentinel](https://github.com/emet-labs/sentinel), built with [Mintlify](https://mintlify.com).

## Development

Install the [Mintlify CLI](https://www.npmjs.com/package/mint) to preview documentation changes locally:

```sh
npm i -g mint
mint dev
```

View the local preview at `http://localhost:3000`.

## Publishing changes

The Mintlify GitHub app is installed on this repo, so changes deploy to production automatically after pushing to the default branch. No build step or CI workflow is required.

### Troubleshooting

- If the dev environment isn't running: run `mint update` to get the most recent CLI version.
- If a page loads as a 404: make sure you're running `mint dev` in the folder with `docs.json`.
