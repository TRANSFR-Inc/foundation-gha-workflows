GitHub Actions reusable workflows by the Foundation team

## How to use
In your workflow, reference at `jobs.<job_name>.uses` as `TRANSFR-Inc/foundation-gha-workflows/.github/workflows/{filename}@{ref}`.

For maximum stability, make the `ref` a sha like so:
```
...
jobs:
  my-job:
    uses: TRANSFR-Inc/foundation-gha-workflows/.github/workflows/ecs-build-and-deploy.yml@abcd0123abcd0123abcd0123abcd0123abcd0123
...
```

For less maintenence, make the `ref` a tag like so:
```
...
jobs:
  my-job:
    uses: TRANSFR-Inc/foundation-gha-workflows/.github/workflows/ecs-build-and-deploy.yml@v0
...
```

Addiontal documentation available here: [reusing-workflows](https://docs.github.com/en/actions/using-workflows/reusing-workflows)
