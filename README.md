# GitHub Self-Hosted Runner

A containerized GitHub Actions runner. Fork of [Pwd9000-ML/docker-github-runner-linux](https://github.com/Pwd9000-ML/docker-github-runner-linux), simplified and published to GitHub Container Registry.

## Usage

```bash
docker run -d \
  -e GH_TOKEN="your-github-token" \
  -e GH_OWNER="your-username" \
  -e GH_REPOSITORY="your-repo" \
  ghcr.io/cswitenky/docker-github-runner-linux:latest
```

## Environment Variables

- `GH_TOKEN` - GitHub Personal Access Token (`repo` and `workflow` scopes)
- `GH_OWNER` - Repository owner
- `GH_REPOSITORY` - Repository name

Works with any GitHub repository. Supports AMD64 and ARM64. 

