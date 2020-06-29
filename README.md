# .NET Core on Google App Engine flexible environment

## Run locally

Build:

```sh
dotnet build
```

Run:

```sh
dotnet run
```

Open in your browser at `http://localhost:8080`

## Deploy to App Engine flexible environment

The [App Engine flexible environment](https://cloud.google.com/appengine/docs/flexible/dotnet) is based on Google Compute Engine and automatically scales your app up and down while balancing the load.

Publish:

```sh
dotnet publish -c Release
```

Deploy:

```sh
gcloud app deploy bin/Release/netcoreapp3.1/publish/app.yaml
```

View:

```sh
gcloud app browse
```
