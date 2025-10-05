# Build the app
docker build -t simplewebserver .

# Run the container
docker run -d -p 8080:80 simplewebserver

# Open network
localhost:8080
