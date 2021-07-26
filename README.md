This app lists out all the 14'ers in Colorado and helps you keep track of when you completed the summit. The original idea was to prepopulate a list of 14'ers which once you check off, it will automatically move the entry from a "to do" list into a "completed" list. Also, there was to allow a single edit button to alter all fields. However, the issue lay in my inability to figure out how to edit multiple properties from a single state (as noted in the NewPeak.js file). Another issue I ran into was using the patch command to replace only the field given. As such, I was only able to update one field.

Code used for formatting from W3 school for bootstrap
Heroku/Netlify tutorial from here: https://www.fabiofranchino.com/blog/how-to-deploy-webapp-heroku-netlify/

Commands run:

Server:
npm init
npm i express pg cors

Database:
docker run --rm --name pg-docker -e POSTGRES_PASSWORD=docker -d -p 5432:5432 -v $HOME/docker/volumes/postgres:/var/lib/postgresql/data postgres
docker ps -a
docker exec -it 2e71fea35d4a bash
psql -U postgres

Client:
npx create-react-app client
npm start