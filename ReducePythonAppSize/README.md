# Build docker image
docker build -t python-script .

# Run container
docker run -v $(pwd)/data:/app/data python-script

# Exit
        a  b  c
count   2  2  2
unique  1  1  1
top     a  b  c
freq    2  2  2
