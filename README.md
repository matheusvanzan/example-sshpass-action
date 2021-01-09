# SSHPASS Github Action

![CI](https://github.com/matheusvanzan/sshpass-action-example/workflows/CI/badge.svg)

Example usage for [sshpass-action](https://github.com/matheusvanzan/sshpass-action)

```
- name: Run sshpass commands
  uses: matheusvanzan/sshpass-action@v2
  with:
    host: ${{ secrets.SERVER_HOST }}
    user: ${{ secrets.SERVER_USER }}
    pass: ${{ secrets.SERVER_PASS }}
    run: |
      # your 
      # commands
      # here
```

Optional ssh port

```
- name: Run sshpass commands
  uses: matheusvanzan/sshpass-action@v2
  with:
    host: ${{ secrets.SERVER_HOST }}
    port: 22
    user: ${{ secrets.SERVER_USER }}
    pass: ${{ secrets.SERVER_PASS }}
    run: |
      # your 
      # commands
      # here
```

Optional private key. In this case it will ignore the password if provided.

```
- name: Run sshpass commands
  uses: matheusvanzan/sshpass-action@v2
  with:
    host: ${{ secrets.SERVER_HOST }}
    user: ${{ secrets.SERVER_USER }}
    key: ${{ secrets.SERVER_KEY }}
    run: |
      # your 
      # commands
      # here
```