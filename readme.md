# Generate a C# Console App
We mount the working directory into `/app` arbitrarily. The dotnet app will be made in the current directory, no extra folders are created.
```bash
docker run --rm -it -v $PWD:/app microsoft/dotnet dotnet new console -o /app
```
# Run The Console App
Run the created app.
```bash
docker run --rm -it -v $PWD:/app microsoft/dotnet dotnet run --project app
```

The location of the project is the directory `app` that's the result of mounting our working directory to `/app` in the container.
