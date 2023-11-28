# demo


## Python 3.9

### init
```bash
sam init --runtime python3.9 --dependency-manager pip --name python --app-template hello-world
```

### build and deploy
```bash
cd python
sam build --use-container && sam deploy --profile personal --no-confirm-changeset
```

### test
```bash
cd python
curl -w "@../curl-format.txt" <API_URL>
```

## Node 20

### init
```bash
sam init --runtime nodejs20.x --dependency-manager npm --name node --app-template hello-world
```

### build and deploy
```bash
cd node
sam build --use-container && sam deploy --profile personal --no-confirm-changeset
```

### test
```bash
cd node
curl -w "@../curl-format.txt" <API_URL>
```


## Java 21

### init
```bash
cd java
sam init --runtime java21 --dependency-manager maven --name java --app-template hello-world
```

### build and deploy
```bash
cd java
sam build --use-container && sam deploy --profile personal --no-confirm-changeset
```

### test
```bash
cd java
curl -w "@../curl-format.txt" <API_URL>
```
