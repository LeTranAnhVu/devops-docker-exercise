```shell script
#build img
docker build -t ex114 .

#run container
docker run  -p 3000:3000 ex114
```

#### edit src:
create file `/config/secrets.yml`:
```yaml
production:
  secret_key_base: <%= ENV["SECRET_KEY_BASE"] %>
```
--> Explain: in order to let the app map secret_key_base ENV variable name

