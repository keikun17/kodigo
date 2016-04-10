# foreman

Start all

     foreman start -f Procfile.dev

Start particular task (ex. client, web, etc)

     foreman start web -f Procfile.dev
     foreman start client -f Procfile.dev

### Procfile format

Example

    web: rails s
    client: sh -c 'rm app/assets/javascripts/generated/* || true && cd client && npm run build:dev:client'
