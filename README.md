# SSHPASS Github Action

![CI](https://github.com/matheusvanzan/sshpass-action-example/workflows/CI/badge.svg)

Example usage for [sshpass-action](https://github.com/matheusvanzan/sshpass-action)

```
- name: Run sshpass commands
  uses: matheusvanzan/sshpass-action@v1
  with:
    host: ${{ secrets.SERVER_HOST }}
    username: ${{ secrets.SERVER_USERNAME }}
    password: ${{ secrets.SERVER_PASSWORD }}
    run: |
      # your 
      # commands
      # here
```
