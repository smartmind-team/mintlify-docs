# ThanoSQL Docs

## Development

Install the [Mintlify CLI](https://www.npmjs.com/package/mintlify) to preview the documentation changes locally. To install, use the following command

```
npm i -g mintlify
```

Run the following command at the root of your documentation (where mint.json is)

```
mintlify dev
```

> [!NOTE]  
> Use dev@smartmind.team as git user.email

## Generating API References

```
npx @mintlify/scraping@latest openapi-file <path-to-openapi-file> -o api-reference
```

then, edit mint.json with navigation object suggestion.

### Troubleshooting

- npm ERR! code EBADENGINE : Update node and npm version.
- Mintlify dev isn't running - Run `mintlify install` it'll re-install dependencies.
- Page loads as a 404 - Make sure you are running in a folder with `mint.json`
