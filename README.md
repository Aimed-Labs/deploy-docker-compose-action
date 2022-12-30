# Example Usage
```yaml
      - name: "Deploy frontend"
        uses: aimed-labs/deploy-docker-compose-action@main
        with:
         working-directory: ./app
         project-name: 'some_app'
         host-address: ${{ secrets.ORG_DEV_SERVER_IP }}
         host-ssh-user: ${{ secrets.ORG_DEV_SERVER_USER }}
         filter: 'label=AIMED_LABS=true'
         ssh-private-key-base64: ${{ secrets.ORG_DEV_SERVER_SSH_PRIVATE_KEY_BASE64 }}
```
