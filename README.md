
### Local Setup
1. `git clone https://github.com/shubhamdhingra38/Spring-Boot-Auction-App.git`
2. Run `cd Spring-Boot-Auction-App/frontend`
3. `git clone https://github.com/shubhamdhingra38/AuctionAppFrontend.git`
4. `mv AuctionAppFrontend app`
5. `cd ..`
6. Download docker if not already
7. Download docker-compose if not already
8. Start docker engine
9. Set up `aws-creds.env` file in the root project directory with your AWS credentials. Leave it empty if you don't want to use upload feature. But file must be created.
10. `docker-compose up --build` inside main directory
11. For a one time setup, you need to create the database `auctionapp`, run `docker exec -it auctionappmysql mysql -u root -p` and enter password as `password`. Then run `CREATE DATABASE auctionapp`. Run `exit`
12. Might need to restart `docker-compose up` again if containers exited, exit and then run `docker-compose up` again
13. Access application on `localhost`


