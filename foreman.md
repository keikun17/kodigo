# foreman

     foreman start -f Procfile.dev


### Procfile format

Example

    web: rails s
    client: sh -c 'rm app/assets/javascripts/generated/* || true && cd client && npm run build:dev:client'
