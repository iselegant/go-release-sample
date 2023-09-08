# go-release-sample

This repository is sample code for automatic release in Go applications.
After modifying the application, by following the steps below, binaries will be automatically generated for each environment via GitHub Actions.

## 1. How to bump up app version as semantic versioning

### bump up major version 
```
make major-version
```

### bump up minor version
```
make minor-version
```

### bump up patch version
```
make patch-version
```

After running these commands, the version variable in main.go will be overwritten.

## 2. Pushing commits and tags after rewriting the version

```
git add .
make push-tag
```
