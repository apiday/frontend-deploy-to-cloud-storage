# Deploy to Cloud Storage action

This action deploys an artifact to Cloud Storage.

## Inputs

### `environment`

The name of the environment to load. Default `""`.
See [`apiday/load-env`](https://github.com/apiday/load-env) action documentation.

## Requirements

This action assumes a GitHub action artifact named was uploaded to `nextjs-build`.
It works well with `apiday/frontend-quality-controls` action.

## Example usage

```
- uses: apiday/frontend-deploy-to-cloud-storage@v1
  with:
    environment: '${{ github.ref_name }}'
```
